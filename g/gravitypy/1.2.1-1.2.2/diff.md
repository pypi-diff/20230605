# Comparing `tmp/gravitypy-1.2.1.tar.gz` & `tmp/gravitypy-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gravitypy-1.2.1.tar", last modified: Thu May 18 21:37:25 2023, max compression
+gzip compressed data, was "gravitypy-1.2.2.tar", last modified: Mon Jun  5 17:34:38 2023, max compression
```

## Comparing `gravitypy-1.2.1.tar` & `gravitypy-1.2.2.tar`

### file list

```diff
@@ -1,29 +1,28 @@
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-18 21:37:25.193660 gravitypy-1.2.1/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1066 2023-05-07 20:40:23.000000 gravitypy-1.2.1/LICENSE
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       25 2023-05-07 20:40:23.000000 gravitypy-1.2.1/MANIFEST.in
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      292 2023-05-18 21:37:25.189660 gravitypy-1.2.1/PKG-INFO
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1332 2023-05-11 15:01:38.000000 gravitypy-1.2.1/README.md
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-18 21:37:25.189660 gravitypy-1.2.1/gravitypy/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 20:40:23.000000 gravitypy-1.2.1/gravitypy/__init__.py
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       70 2023-05-12 13:14:06.000000 gravitypy-1.2.1/gravitypy/__main__.py
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-18 21:37:25.189660 gravitypy-1.2.1/gravitypy/button/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       27 2023-05-12 13:07:34.000000 gravitypy-1.2.1/gravitypy/button/__init__.py
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     2188 2023-05-18 21:36:27.000000 gravitypy-1.2.1/gravitypy/button/button.py
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-05-18 19:07:09.000000 gravitypy-1.2.1/gravitypy/config.py
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)    13251 2023-05-18 21:36:34.000000 gravitypy-1.2.1/gravitypy/main.py
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-18 21:37:25.189660 gravitypy-1.2.1/gravitypy/particle/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       31 2023-05-12 13:07:49.000000 gravitypy-1.2.1/gravitypy/particle/__init__.py
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     5394 2023-05-18 20:27:42.000000 gravitypy-1.2.1/gravitypy/particle/particle.py
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-18 21:37:25.189660 gravitypy-1.2.1/gravitypy/resources/
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-18 21:37:25.189660 gravitypy-1.2.1/gravitypy/resources/fonts/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)    15700 2023-05-07 20:40:23.000000 gravitypy-1.2.1/gravitypy/resources/fonts/minecraft_font.ttf
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-18 21:37:25.189660 gravitypy-1.2.1/gravitypy.egg-info/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      292 2023-05-18 21:37:25.000000 gravitypy-1.2.1/gravitypy.egg-info/PKG-INFO
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      500 2023-05-18 21:37:25.000000 gravitypy-1.2.1/gravitypy.egg-info/SOURCES.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-05-18 21:37:25.000000 gravitypy-1.2.1/gravitypy.egg-info/dependency_links.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       54 2023-05-18 21:37:25.000000 gravitypy-1.2.1/gravitypy.egg-info/entry_points.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       14 2023-05-18 21:37:25.000000 gravitypy-1.2.1/gravitypy.egg-info/requires.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       10 2023-05-18 21:37:25.000000 gravitypy-1.2.1/gravitypy.egg-info/top_level.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       14 2023-05-07 20:40:23.000000 gravitypy-1.2.1/requirements.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       38 2023-05-18 21:37:25.193660 gravitypy-1.2.1/setup.cfg
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      959 2023-05-18 21:36:45.000000 gravitypy-1.2.1/setup.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-06-05 17:34:38.135845 gravitypy-1.2.2/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1066 2023-05-07 20:40:23.000000 gravitypy-1.2.2/LICENSE
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       25 2023-05-07 20:40:23.000000 gravitypy-1.2.2/MANIFEST.in
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      292 2023-06-05 17:34:38.135845 gravitypy-1.2.2/PKG-INFO
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1480 2023-06-05 17:20:56.000000 gravitypy-1.2.2/README.md
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-06-05 17:34:38.131845 gravitypy-1.2.2/gravitypy/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 20:40:23.000000 gravitypy-1.2.2/gravitypy/__init__.py
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       70 2023-05-12 13:14:06.000000 gravitypy-1.2.2/gravitypy/__main__.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-06-05 17:34:38.135845 gravitypy-1.2.2/gravitypy/button/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       27 2023-05-12 13:07:34.000000 gravitypy-1.2.2/gravitypy/button/__init__.py
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     2695 2023-06-05 17:14:48.000000 gravitypy-1.2.2/gravitypy/button/button.py
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)    14366 2023-06-05 17:26:16.000000 gravitypy-1.2.2/gravitypy/main.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-06-05 17:34:38.135845 gravitypy-1.2.2/gravitypy/particle/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       31 2023-05-12 13:07:49.000000 gravitypy-1.2.2/gravitypy/particle/__init__.py
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     6138 2023-05-27 20:03:20.000000 gravitypy-1.2.2/gravitypy/particle/particle.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-06-05 17:34:38.131845 gravitypy-1.2.2/gravitypy/resources/
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-06-05 17:34:38.135845 gravitypy-1.2.2/gravitypy/resources/fonts/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)    15700 2023-05-07 20:40:23.000000 gravitypy-1.2.2/gravitypy/resources/fonts/minecraft_font.ttf
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-06-05 17:34:38.131845 gravitypy-1.2.2/gravitypy.egg-info/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      292 2023-06-05 17:34:38.000000 gravitypy-1.2.2/gravitypy.egg-info/PKG-INFO
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      480 2023-06-05 17:34:38.000000 gravitypy-1.2.2/gravitypy.egg-info/SOURCES.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-06-05 17:34:38.000000 gravitypy-1.2.2/gravitypy.egg-info/dependency_links.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       54 2023-06-05 17:34:38.000000 gravitypy-1.2.2/gravitypy.egg-info/entry_points.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       14 2023-06-05 17:34:38.000000 gravitypy-1.2.2/gravitypy.egg-info/requires.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       10 2023-06-05 17:34:38.000000 gravitypy-1.2.2/gravitypy.egg-info/top_level.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       14 2023-05-07 20:40:23.000000 gravitypy-1.2.2/requirements.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       38 2023-06-05 17:34:38.135845 gravitypy-1.2.2/setup.cfg
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      959 2023-06-05 17:27:53.000000 gravitypy-1.2.2/setup.py
```

### Comparing `gravitypy-1.2.1/LICENSE` & `gravitypy-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gravitypy-1.2.1/README.md` & `gravitypy-1.2.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+
+![up (1)](https://github.com/WiktorK02/gravitypy/assets/123249470/bba03417-8be4-4270-9402-741e3c763355)
 # GravityPy
 ## About Project
-Simulation presents full customizable n-body problem using pygame
+GravityPy is a high-performance pygame application presenting a fully customizable n-body gravity simulation
 ## Getting Started
 ### Prerequisites
 Download python, pip and check version
 ```
 $ pip3 --version 
 $ python --version
 ```
```

### Comparing `gravitypy-1.2.1/gravitypy/button/button.py` & `gravitypy-1.2.2/gravitypy/button/button.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         self.text_input = text_input
         self.button_rect = button_rect
         self.text = font.render(self.text_input, True, "white")
         self.text_rect = self.text.get_rect(center=(self.button_rect.center))
         self.surface = pygame.Surface(self.button_rect.size, pygame.SRCALPHA) 
         self.color = (100, 80, 90, 128)  # Set the color with transparency
         
-    def draw(self, screen):   
+    def draw(self, screen): 
         pygame.draw.rect(self.surface, self.color, (0, 0, *self.button_rect.size))  
         screen.blit(self.surface, self.button_rect)  
         screen.blit(self.text, self.text_rect)
     
     def decrease_radius(self, added_radius):
         if added_radius > 1:
             return added_radius - 1
@@ -46,17 +46,29 @@
         added_velocity.y -= 0.05
         return added_velocity
 
     def increase_velocity_y(self, added_velocity, add_button_statement_put):
         added_velocity.y += 0.05
         return added_velocity
 
-    def reset_particles(self, num_particles, particles, reset_button_statement):
-        num_particles = 0
-        particles = []
+    def reset_particles(self, num_particles, particles, reset_button_statement, hide_button):
+        if not hide_button:    
+            num_particles = 0
+            particles = []
         reset_button_statement = False
         return num_particles, particles, reset_button_statement
 
-    def reset_scale(self, scale, reset_scale_button_statement):
-        scale = 1.0
-        reset_scale_button_statement = False
-        return scale, reset_scale_button_statement 
+    def reset_scale(self, scale, reset_scale_button_statement, hide_button):
+        if not hide_button:    
+            scale = 1.0
+            reset_scale_button_statement = False
+        return scale, reset_scale_button_statement 
+    
+    def reset_vel(self, vel, reset_button_statement):
+        vel = pygame.Vector2(0, 0)
+        reset_button_statement = False
+        return vel, reset_button_statement
+   
+    def change_text(self, text_input, font):
+        self.text_input = text_input
+        self.text = font.render(self.text_input, True, "white")
+        self.text_rect = self.text.get_rect(center=self.button_rect.center)
```

### Comparing `gravitypy-1.2.1/gravitypy/main.py` & `gravitypy-1.2.2/gravitypy/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,22 +15,22 @@
     font_file = os.path.join(current_dir, 'resources', 'fonts', 'minecraft_font.ttf')
     font_size = 16
     FONT = pygame.font.Font(font_file, font_size)
 
     WIDTH, HEIGHT = 1200, 700
     SCREEN = pygame.display.set_mode((WIDTH, HEIGHT))
     CLOCK = pygame.time.Clock()
-    G = 100
+    G = 1
     SCALE = 1.0
     PARTICLES = []
-    ADDED_RADIUS = 20
-    ADDED_MASS = 20
+    ADDED_RADIUS = 5
+    ADDED_MASS = 5
     ADDED_VELOCITY = pygame.Vector2(0, 0)
-    NUM_PARTICLES = 40
-    ADDED_COLOR = (random.randint(0, 255), random.randint(0, 255), random.randint(0, 255))
+    NUM_PARTICLES = 250
+    ADDED_COLOR = (255,255,255)
     MOUSE_X, MOUSE_Y = pygame.mouse.get_pos()
     
     # Initialize states  
     states = {
         'increase_radius':          False,
         'decrease_radius':          False,
         'increase_mass':            False,
@@ -39,81 +39,105 @@
         'decrease_velocity_x':      False,
         'increase_velocity_y':      False,
         'decrease_velocity_y':      False,
         'add_particle':             False,
         'add_particle_put':         False,
         'reset_particles':          False,
         'reset_scale':              False,
+        'reset_vel':                False,
         'move_particles':           False,
-        'pause':                    False
+        'pause':                    False,
+        'hide_button':              False
+
+
     }
     
     # Initialize Buttons
     buttons = {
         'button_increase_r':  Buttons(50,50,"Increse R", pygame.Rect(50,50,120,25), FONT),
         'button_decrease_r':  Buttons(150,50,"Decrese R", pygame.Rect(50,85,120,25), FONT),
         'button_increase_m':  Buttons(250,50,"Increse M", pygame.Rect(200,50,120,25), FONT),
         'button_decrease_m':  Buttons(350,50,"Decrese M", pygame.Rect(200,85,120,25), FONT),
         'button_increase_vx': Buttons(250,50,"+ Vx", pygame.Rect(350,50,50,25), FONT),
         'button_decrease_vx': Buttons(350,50,"- Vx", pygame.Rect(350,85,50,25), FONT),
         'button_increase_vy': Buttons(250,50,"+ Vy", pygame.Rect(410,50,50,25), FONT),
         'button_decrease_vy': Buttons(350,50,"- Vy", pygame.Rect(410,85,50,25), FONT),
-        'add_button':         Buttons(350,50,"Add", pygame.Rect(550,50,120,60), FONT),
+        'button_res_vel':     Buttons(350,50,"Res vel", pygame.Rect(480,50,50,60), FONT),
+        'add_button':         Buttons(350,50,"Add particle", pygame.Rect(550,50,140,60), FONT),
         'reset_button':       Buttons(350,50,"Reset Praticles", pygame.Rect(850,50,160,25), FONT),
-        'reset_scale_button': Buttons(350,50,"Reset scale", pygame.Rect(1050,50,120,25), FONT)
+        'reset_scale_button': Buttons(350,50,"Reset scale", pygame.Rect(1050,50,120,25), FONT),
+        'hide_button':        Buttons(350,50,"Hide buttons", pygame.Rect(1030,650,150,25), FONT)       
     }
-    
-    # Generate random particles
+      
+    # Generate random particlesbutton
     for i in range(NUM_PARTICLES):
         if i == 0:
             x = WIDTH // 2
             y = HEIGHT// 2
-            mass = 60
-            PARTICLES.append(Particles(x, y, mass, (random.randint(0, 255), random.randint(0, 255), random.randint(0, 255)), random.randint(30, 30), pygame.Vector2(0, 0)))
+            mass = 10000
+            radius = random.randint(10, 10)
+            PARTICLES.append(Particles(x, y, mass, (189, 255, 20) , radius, pygame.Vector2(0, 0)))
         else:
-            x = random.randint(0, WIDTH)
-            y = random.randint(0, HEIGHT)
-            mass = random.uniform(1, 10)
-            mass = 5
-            PARTICLES.append(Particles(x, y, mass, (random.randint(0, 255), random.randint(0, 255), random.randint(0, 255)), random.randint(0, 5), pygame.Vector2(0, 0)))
+            x =  i*3
+            y = 100 
+            mass = int(random.uniform(1, 10))
+            radius = int(random.randint(1, 3))
+            PARTICLES.append(Particles(x, y, mass, (255,255,255), radius, pygame.Vector2(2.0, 0)))
 
     running = True
 
     while running:
         for event in pygame.event.get():
             if event.type == pygame.QUIT:
                 running = False
             elif event.type == pygame.MOUSEBUTTONDOWN:
                 
                 # Left click
                 if event.button == 1: 
                     if buttons['button_increase_r'].button_rect.collidepoint(event.pos):
                         states['increase_radius'] = True
+
                     elif buttons['button_decrease_r'].button_rect.collidepoint(event.pos):
                         states['decrease_radius'] = True
+
                     elif buttons['button_increase_m'].button_rect.collidepoint(event.pos):
                         states['increase_mass'] = True
+
                     elif buttons['button_decrease_m'].button_rect.collidepoint(event.pos):
                         states['decrease_mass'] = True
+
                     elif buttons['button_increase_vx'].button_rect.collidepoint(event.pos):
                         states['increase_velocity_x'] = True
+
                     elif buttons['button_decrease_vx'].button_rect.collidepoint(event.pos):
                         states['decrease_velocity_x'] = True
+
                     elif buttons['button_increase_vy'].button_rect.collidepoint(event.pos):
                         states['increase_velocity_y'] = True
+
                     elif buttons['button_decrease_vy'].button_rect.collidepoint(event.pos):
                         states['decrease_velocity_y'] = True
+
                     elif buttons['add_button'].button_rect.collidepoint(event.pos):
                         states['add_particle'] = True
+
                     elif states['add_particle']:
                         states['add_particle_put'] = True
+
                     elif buttons['reset_button'].button_rect.collidepoint(event.pos):
                         states['reset_particles'] = True
+
                     elif buttons['reset_scale_button'].button_rect.collidepoint(event.pos):
                         states['reset_scale'] = True
+
+                    elif buttons['hide_button'].button_rect.collidepoint(event.pos):
+                        states['hide_button'] = not states['hide_button']
+                    
+                    elif buttons['button_res_vel'].button_rect.collidepoint(event.pos):
+                        states['reset_vel'] = not states['reset_vel']
                     
                     for particle in PARTICLES:
                         scaled_x = int(MOUSE_X + (particle.position.x - MOUSE_X) * SCALE)
                         scaled_y = int(MOUSE_Y + (particle.position.y - MOUSE_Y) * SCALE)
                         distance = math.sqrt((event.pos[0] - scaled_x)**2 + (event.pos[1] - scaled_y)**2)
                         if distance <= particle.radius * SCALE:
                             particle.selected = not particle.selected
@@ -133,47 +157,82 @@
                     if SCALE - 0.1 > 0:
                         SCALE -= 0.1
                         MOUSE_X, MOUSE_Y = pygame.mouse.get_pos()
                     
             elif event.type == pygame.MOUSEBUTTONUP:
                 if event.button == 1:
                     # Reset button states
-                    states['increase_radius'] = False
-                    states['decrease_radius'] = False
-                    states['increase_mass'] = False
-                    states['decrease_mass'] = False
+                    states['increase_radius']     = False
+                    states['decrease_radius']     = False
+                    states['increase_mass']       = False
+                    states['decrease_mass']       = False
                     states['increase_velocity_x'] = False
                     states['decrease_velocity_x'] = False
                     states['increase_velocity_y'] = False
                     states['decrease_velocity_y'] = False
-                    states['add_button'] = False
-                    states['reset_partilces'] = False
-                    states['reset_scale'] = False
+                    states['add_button']          = False
+                    states['reset_partilces']     = False
+                    states['reset_scale']         = False
                     
             elif event.type == pygame.KEYDOWN:
                 if event.key == pygame.K_LEFT:
                     states['move_particles'] = True
                     move_direction = pygame.Vector2(5/SCALE, 0)
+
                 elif event.key == pygame.K_RIGHT:
                     states['move_particles'] = True
                     move_direction = pygame.Vector2(-5/SCALE, 0)
+
                 elif event.key == pygame.K_UP:
                     states['move_particles'] = True
                     move_direction = pygame.Vector2(0, 5/SCALE)
+
                 elif event.key == pygame.K_DOWN:
                     states['move_particles'] = True
                     move_direction = pygame.Vector2(0, -5/SCALE)
+
                 elif event.key == pygame.K_SPACE:
                     states['pause'] = not states['pause']
             
             elif event.type == pygame.KEYUP:
                 if event.key in [pygame.K_LEFT, pygame.K_RIGHT, pygame.K_UP, pygame.K_DOWN]:
                     states['move_particles'] = False
 
-        SCREEN.fill((20,20,40))
+        SCREEN.fill((9, 20, 20))
+        
+        text_data = {
+            'text_radius': {
+                'text': FONT.render(f'Radius: {ADDED_RADIUS}', True, (240, 240, 240)),
+                'position': (50, 20)
+            },
+            'text_mass': {
+                'text': FONT.render(f'Mass: {ADDED_MASS}', True, (240, 240, 240)),
+                'position': (200, 20)
+            },
+            'text_velocity': {
+                'text': FONT.render(f'Velocity: {ADDED_VELOCITY}', True, (240, 240, 240)),
+                'position': (350, 20)
+            },
+            'text_num_particles': {
+                'text': FONT.render(f'Number of particles: {NUM_PARTICLES}', True, (240, 240, 240)),
+                'position': (950, 0)
+            },
+            'text_scale': {
+                'text': FONT.render(f'Scale: {int(SCALE * 100)}%', True, (240, 240, 240)),
+                'position': (950, 20)
+            },
+            'text_info': {
+                'text': FONT.render('Move camera with arrow keys, pause with a space', True, (240, 240, 240)),
+                'position': (700, 85)
+            },
+            'text_fps': {
+                'text': FONT.render("FPS: {:.2f}".format(CLOCK.get_fps()), True, (255, 255, 255)),
+                'position': (1070, 20)
+            }
+        }
 
         if states['increase_radius']:
             ADDED_RADIUS = buttons['button_increase_r'].increase_radius(ADDED_RADIUS)
         elif states['decrease_radius']:
             ADDED_RADIUS = buttons['button_decrease_r'].decrease_radius(ADDED_RADIUS)
         elif states['increase_mass']:
             ADDED_MASS = buttons['button_increase_m'].increase_mass(ADDED_MASS)
@@ -184,17 +243,36 @@
         elif states['decrease_velocity_x']:
             ADDED_VELOCITY = buttons['button_decrease_vx'].decrease_velocity_x(ADDED_VELOCITY, states['add_particle'])
         elif states['increase_velocity_y']:
             ADDED_VELOCITY = buttons['button_increase_vy'].increase_velocity_y(ADDED_VELOCITY, states['add_particle'])
         elif states['decrease_velocity_y']:
             ADDED_VELOCITY = buttons['button_decrease_vx'].decrease_velocity_y(ADDED_VELOCITY, states['add_particle'])
         elif states['reset_particles']:
-            NUM_PARTICLES, PARTICLES, states['reset_particles'] = buttons['reset_button'].reset_particles(NUM_PARTICLES, PARTICLES, states['reset_particles'])
+            NUM_PARTICLES, PARTICLES, states['reset_particles'] = buttons['reset_button'].reset_particles(NUM_PARTICLES, PARTICLES, states['reset_particles'], states['hide_button'])
         elif states['reset_scale']:
-            SCALE, states['reset_scale'] = buttons['reset_scale_button'].reset_scale(SCALE, states['reset_scale'])
+            SCALE, states['reset_scale'] = buttons['reset_scale_button'].reset_scale(SCALE, states['reset_scale'], states['hide_button'])
+        elif states['reset_vel']:
+            ADDED_VELOCITY, states['reset_vel'] = buttons['button_res_vel'].reset_vel(ADDED_VELOCITY, states['reset_vel'])
+        
+        # Hide or unhide buttons 
+        if states['hide_button']:
+            for button_name, button in buttons.items():
+                if button_name == 'hide_button':
+                    button.change_text('unhide buttons', FONT)
+                    button.draw(SCREEN) 
+            for data in text_data.values():
+                data.pop('text', None)
+        else:
+            for button_name, button in buttons.items():
+                if button_name == 'hide_button':
+                    button.change_text('hide buttons', FONT)
+                button.draw(SCREEN)
+            for key, data in text_data.items():
+                SCREEN.blit(data['text'], data['position'])
+
 
         if states['add_particle']:
             actual_mouse_x, actuale_mouse_y = pygame.mouse.get_pos()
             scaled_mouse_x = int(MOUSE_X + (actual_mouse_x - MOUSE_X) * SCALE)
             scaled_mouse_y = int(MOUSE_Y + (actuale_mouse_y - MOUSE_Y) * SCALE)
             circle_center = (scaled_mouse_x, scaled_mouse_y)
             circle_radius = int(ADDED_RADIUS * SCALE)
@@ -216,15 +294,15 @@
                     ADDED_COLOR ,
                     ADDED_RADIUS,
                     particle_velocity
                 )
             )
             states['add_particle_put'] = False
             # Change color of the next particle
-            ADDED_COLOR  = (random.randint(0, 255), random.randint(0, 255), random.randint(0, 255))
+            ADDED_COLOR  = (255,255,255)
             NUM_PARTICLES += 1
 
         # Sort in case bigger particles do not cover smaller ones 
         PARTICLES = sorted(PARTICLES, key=lambda x: x.radius, reverse=True)
         
         boundary = pygame.Rect(0, 0, WIDTH, HEIGHT)
         capacity = 4  
@@ -236,52 +314,11 @@
         for particle in PARTICLES:
             if states['move_particles']:
                 particle.position += move_direction * SCALE
             elif not states['pause']:
                 particle.update()
                 quadtree.calculate_forces(particle, G)
             particle.draw_scaled(MOUSE_X, MOUSE_Y, SCALE, WIDTH, HEIGHT, SCREEN, FONT)
-    
-        # Draw Buttons
-        for button_name, button in buttons.items():
-            button.draw(SCREEN)
-        
-        text_data = {
-            'text_radius': {
-                'text': FONT.render(f'Radius: {ADDED_RADIUS}', True, (240, 240, 240)),
-                'position': (50, 20)
-            },
-            'text_mass': {
-                'text': FONT.render(f'Mass: {ADDED_MASS}', True, (240, 240, 240)),
-                'position': (200, 20)
-            },
-            'text_velocity': {
-                'text': FONT.render(f'Velocity: {ADDED_VELOCITY}', True, (240, 240, 240)),
-                'position': (350, 20)
-            },
-            'text_num_particles': {
-                'text': FONT.render(f'Number of particles: {NUM_PARTICLES}', True, (240, 240, 240)),
-                'position': (950, 0)
-            },
-            'text_scale': {
-                'text': FONT.render(f'Scale: {int(SCALE * 100)}%', True, (240, 240, 240)),
-                'position': (950, 20)
-            },
-            'text_info': {
-                'text': FONT.render('Move camera with arrow keys, pause with a space', True, (240, 240, 240)),
-                'position': (700, 85)
-            },
-            'text_fps': {
-                'text': FONT.render("FPS: {:.2f}".format(CLOCK.get_fps()), True, (255, 255, 255)),
-                'position': (1070, 20)
-            }
-        }
-       
-        # Draw text 
-        for key, data in text_data.items():
-            SCREEN.blit(data['text'], data['position'])
-    
 
         pygame.display.update()
         CLOCK.tick(60)
-    
-    pygame.quit()
+    pygame.quit()
```

### Comparing `gravitypy-1.2.1/gravitypy/particle/particle.py` & `gravitypy-1.2.2/gravitypy/particle/particle.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import pygame
 import math
+from collections import deque
 
 class QuadTree:
     def __init__(self, boundary, capacity):
         self.boundary = boundary
         self.capacity = capacity
         self.particles = []
         self.is_divided = False
@@ -89,28 +90,31 @@
         self.position = pygame.Vector2(x, y)
         self.velocity = velocity
         self.mass = mass
         self.radius = radius
         self.color = color
         self.stats_text = None
         self.selected = None
+        self.path = deque(maxlen=100)  # Maximum length of the path
 
     def apply_force(self, force):
         acceleration = force / self.mass
         self.velocity += acceleration
 
     def update(self):
         self.position += self.velocity
+        self.path.append(self.position.copy())  # Add current position to the path
 
     def draw_scaled(self, mouse_x, mouse_y, scale, width, height, screen, font):
         scaled_x = int(mouse_x + (self.position.x - mouse_x) * scale)
         scaled_y = int(mouse_y + (self.position.y - mouse_y) * scale)
         circle_center = (scaled_x, scaled_y)
         radius_scaled = int(self.radius * scale)
 
+        # Draw the particle if it is within the screen boundaries
         if 0 < scaled_y < height and 0 < scaled_x < width:
             pygame.draw.circle(screen, self.color, circle_center, radius_scaled)
 
         # Render and position the statistics text
         if self.selected:
             text_y = scaled_y + radius_scaled + 10
             stats_lines = [
@@ -120,11 +124,21 @@
             ]
             line_height = 20
             stats_surfaces = [font.render(line, True, (255, 255, 255)) for line in stats_lines]
 
             for i, stats_text in enumerate(stats_surfaces):
                 stats_text_rect = stats_text.get_rect(center=(scaled_x, text_y + i * line_height))
                 screen.blit(stats_text, stats_text_rect)
+                        # Add the current position to the path (unscaled)
+            self.path.append(self.position.copy())
+
+            # Scale the path coordinates
+            scaled_path = [(int(mouse_x + (pos.x - mouse_x) * scale), int(mouse_y + (pos.y - mouse_y) * scale))
+                        for pos in self.path]
+
+            # Draw the path if it has at least two points
+            if len(scaled_path) >= 16:
+                pygame.draw.lines(screen, self.color, False, scaled_path)
 
     def is_clicked(self, mouse_pos):
         squared_distance = self.position.distance_squared_to(pygame.Vector2(*mouse_pos))
         return squared_distance <= self.radius**2
```

### Comparing `gravitypy-1.2.1/gravitypy/resources/fonts/minecraft_font.ttf` & `gravitypy-1.2.2/gravitypy/resources/fonts/minecraft_font.ttf`

 * *Files identical despite different names*

### Comparing `gravitypy-1.2.1/setup.py` & `gravitypy-1.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 req_file = os.path.join(here, 'requirements.txt')
 with open(req_file, 'r') as f:
     REQUIREMENTS = [line.strip() for line in f.readlines()]
 LONG_DESCRIPTION = 'Pygame N-Body gravity simulation app'
 
 setup(
    name='gravitypy',
-   version='1.2.1',
+   version='1.2.2',
    description='GravityPy',
    license="MIT",
    author='WiktorK02',
    author_email='wiktor.kidon@hotmail.com',
    url="https://github.com/WiktorK02/gravityPy",
    long_description_content_type="text/markdown",
    package_data={'gravitypy': ['*']},
```

