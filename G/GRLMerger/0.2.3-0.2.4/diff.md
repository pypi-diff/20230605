# Comparing `tmp/GRLMerger-0.2.3-py3-none-any.whl.zip` & `tmp/GRLMerger-0.2.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 29234 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat   224869 b- defN 23-Jun-05 19:44 grlmerger.py
--rw-rw-rw-  2.0 fat     1247 b- defN 23-Jun-05 19:48 GRLMerger-0.2.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-05 19:48 GRLMerger-0.2.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 23-Jun-05 19:48 GRLMerger-0.2.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      377 b- defN 23-Jun-05 19:48 GRLMerger-0.2.3.dist-info/RECORD
-5 files, 226595 bytes uncompressed, 28536 bytes compressed:  87.4%
+Zip file size: 29229 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat   224905 b- defN 23-Jun-05 19:52 grlmerger.py
+-rw-rw-rw-  2.0 fat     1247 b- defN 23-Jun-05 19:52 GRLMerger-0.2.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-05 19:52 GRLMerger-0.2.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-Jun-05 19:52 GRLMerger-0.2.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      377 b- defN 23-Jun-05 19:52 GRLMerger-0.2.4.dist-info/RECORD
+5 files, 226631 bytes uncompressed, 28531 bytes compressed:  87.4%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: grlmerger.py
 Comment: 
 
-Filename: GRLMerger-0.2.3.dist-info/METADATA
+Filename: GRLMerger-0.2.4.dist-info/METADATA
 Comment: 
 
-Filename: GRLMerger-0.2.3.dist-info/WHEEL
+Filename: GRLMerger-0.2.4.dist-info/WHEEL
 Comment: 
 
-Filename: GRLMerger-0.2.3.dist-info/top_level.txt
+Filename: GRLMerger-0.2.4.dist-info/top_level.txt
 Comment: 
 
-Filename: GRLMerger-0.2.3.dist-info/RECORD
+Filename: GRLMerger-0.2.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## grlmerger.py

```diff
@@ -3166,21 +3166,21 @@
         merged_relations_df_copy['parent_element_ID'][i] = re.sub('[+]', '', merged_relations_df_copy['parent_element_ID'][i])
         merged_relations_df_copy['child_actor_ID'][i] = re.sub('[+]', '', merged_relations_df_copy['child_actor_ID'][i])
         merged_relations_df_copy['child_element_ID'][i] = re.sub('[+]', '', merged_relations_df_copy['child_element_ID'][i])
         merged_relations_df_copy['relation_ID'][i] = re.sub('[+]', '', merged_relations_df_copy['relation_ID'][i])
         
     mergedActorsIDs_copy = merged_actors_df_copy['actor_ID'].to_list()
     
-    global model_1_name
-    global model_2_name
+    global input_model_a_name
+    global input_model_b_name
     mergedActorsIDs_copy.append('X#Y')
     tgrlList = []
     p = re.compile('\d+(\.\d+)?')
     # process dummy actors differently
-    tgrlList.append("grl mergedModel_"+model_1_name+"_"+model_2_name+" {")
+    tgrlList.append("grl mergedModel_"+input_model_a_name+"_"+input_model_b_name+" {")
     for i in range(len(mergedActorsIDs_copy)):
         currentMergedActor = pd.DataFrame(merged_actors_df_copy.loc[merged_actors_df_copy['actor_ID'] == mergedActorsIDs_copy[i]])
         if mergedActorsIDs_copy[i] != 'X#Y':
             tgrlList.append('actor '+ mergedActorsIDs_copy[i] + " {")
             if currentMergedActor['actor_name'].item() != "":
                 tgrlList.append('name = \"' + currentMergedActor['actor_name'].item() + '\";')
             if currentMergedActor['actor_description'].item() != "": 
@@ -3261,15 +3261,15 @@
                     tgrlList.append(relation + " {" + str(contributionValue) + ";};")
                 else:
                     tgrlList.append(relation + ";")
         if mergedActorsIDs_copy[i] != 'X#Y':
             tgrlList.append('}') #closing the actor
     tgrlList.append('}') #closing the model
 
-    integratedModel_fileName = 'integratedModel_'+model_1_name+'_'+model_2_name+'_indirect_cycles.xgrl'
+    integratedModel_fileName = 'integratedModel_'+input_model_a_name+'_'+input_model_b_name+'_indirect_cycles.xgrl'
 
     with open(integratedModel_fileName, 'w') as filehandle:
         for listitem in tgrlList:
             filehandle.write('%s\n' % listitem)
```

## Comparing `GRLMerger-0.2.3.dist-info/METADATA` & `GRLMerger-0.2.4.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GRLMerger
-Version: 0.2.3
+Version: 0.2.4
 Summary: GRL Merger is a package that integrates two GRL models written in TGRL syntax into one GRL model.
 Home-page: UNKNOWN
 Author: GRLMerger Authors
 Author-email: <g201906430@gmail.com>
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

