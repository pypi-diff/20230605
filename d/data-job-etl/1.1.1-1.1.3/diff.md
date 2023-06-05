# Comparing `tmp/data_job_etl-1.1.1-py3-none-any.whl.zip` & `tmp/data_job_etl-1.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 212293 bytes, number of entries: 26
+Zip file size: 213341 bytes, number of entries: 26
 -rw-r--r--  2.0 unx     4480 b- defN 80-Jan-01 00:00 data_job_etl/.ipynb_checkpoints/rank-checkpoint.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 data_job_etl/__init__.py
 -rw-r--r--  2.0 unx    75536 b- defN 80-Jan-01 00:00 data_job_etl/analysis.ipynb
 -rw-r--r--  2.0 unx     3487 b- defN 80-Jan-01 00:00 data_job_etl/build_technos.py
 -rw-r--r--  2.0 unx      371 b- defN 80-Jan-01 00:00 data_job_etl/config/definitions.py
 -rw-r--r--  2.0 unx      486 b- defN 80-Jan-01 00:00 data_job_etl/config/etl_logger.py
 -rw-r--r--  2.0 unx     2300 b- defN 80-Jan-01 00:00 data_job_etl/config/postgres_schema.py
@@ -12,17 +12,17 @@
 -rw-r--r--  2.0 unx     1363 b- defN 80-Jan-01 00:00 data_job_etl/etl.py
 -rw-r--r--  2.0 unx      418 b- defN 80-Jan-01 00:00 data_job_etl/extract/extract.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 data_job_etl/file.log
 -rw-r--r--  2.0 unx      380 b- defN 80-Jan-01 00:00 data_job_etl/load/create_tables.py
 -rw-r--r--  2.0 unx     4661 b- defN 80-Jan-01 00:00 data_job_etl/load/load.py
 -rw-r--r--  2.0 unx     5979 b- defN 80-Jan-01 00:00 data_job_etl/message.py
 -rw-r--r--  2.0 unx     4480 b- defN 80-Jan-01 00:00 data_job_etl/rank.py
--rw-r--r--  2.0 unx     3040 b- defN 80-Jan-01 00:00 data_job_etl/recommendation_system.py
+-rw-r--r--  2.0 unx     8076 b- defN 80-Jan-01 00:00 data_job_etl/recommendation_system.py
 -rw-r--r--  2.0 unx     2547 b- defN 80-Jan-01 00:00 data_job_etl/summarise.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 data_job_etl/transform/file.log
--rw-r--r--  2.0 unx     1965 b- defN 80-Jan-01 00:00 data_job_etl/transform/preprocess.py
+-rw-r--r--  2.0 unx     1991 b- defN 80-Jan-01 00:00 data_job_etl/transform/preprocess.py
 -rw-r--r--  2.0 unx     2254 b- defN 80-Jan-01 00:00 data_job_etl/transform/process.py
--rw-r--r--  2.0 unx     1641 b- defN 80-Jan-01 00:00 data_job_etl/update_table.py
--rw-r--r--  2.0 unx      465 b- defN 80-Jan-01 00:00 data_job_etl-1.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 data_job_etl-1.1.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx     2203 b- defN 16-Jan-01 00:00 data_job_etl-1.1.1.dist-info/RECORD
-26 files, 918420 bytes uncompressed, 208711 bytes compressed:  77.3%
+-rw-r--r--  2.0 unx     1674 b- defN 80-Jan-01 00:00 data_job_etl/update_table.py
+-rw-r--r--  2.0 unx      465 b- defN 80-Jan-01 00:00 data_job_etl-1.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 data_job_etl-1.1.3.dist-info/WHEEL
+?rw-r--r--  2.0 unx     2203 b- defN 16-Jan-01 00:00 data_job_etl-1.1.3.dist-info/RECORD
+26 files, 923515 bytes uncompressed, 209759 bytes compressed:  77.3%
```

## zipnote {}

```diff
@@ -63,17 +63,17 @@
 
 Filename: data_job_etl/transform/process.py
 Comment: 
 
 Filename: data_job_etl/update_table.py
 Comment: 
 
-Filename: data_job_etl-1.1.1.dist-info/METADATA
+Filename: data_job_etl-1.1.3.dist-info/METADATA
 Comment: 
 
-Filename: data_job_etl-1.1.1.dist-info/WHEEL
+Filename: data_job_etl-1.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: data_job_etl-1.1.1.dist-info/RECORD
+Filename: data_job_etl-1.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## data_job_etl/recommendation_system.py

```diff
@@ -1,105 +1,184 @@
 import os
+import re
 import pandas as pd
 import numpy as np
 from sklearn.feature_extraction.text import CountVectorizer
 from sklearn.metrics.pairwise import cosine_similarity
 from sqlalchemy import create_engine
 
 USER = os.getenv('JOB_MARKET_DB_USER')
 PWD = os.getenv('JOB_MARKET_DB_PWD')
 
 pd.options.mode.chained_assignment = None
 pd.reset_option('display.max_rows')
 pd.set_option('display.max_rows', 500)
 
 
-def extract_data():
-    engine = create_engine(f"postgresql://{USER}:{PWD}@localhost:5432/job_market")
-    query = 'SELECT * FROM relevant;'
-    relevant = pd.read_sql_query(query, engine)
-    relevant = relevant[
-        ['id', 'title', 'company', 'remote', 'location', 'stack', 'education', 'size', 'experience', 'rank', 'url',
-         'industry', 'type', 'created_at', 'text', 'summary']]
-    # print(relevant.info())
+class Recommender:
+    def __init__(self, job_id, columns=None, feature_columns=None, feature_names_weights=None):
+        self.job_id = job_id
+        if columns is None:
+            self.columns = ['id', 'title', 'company', 'remote', 'location', 'stack', 'text', 'experience', 'size']
+        else:
+            self.columns = columns
+        if feature_columns is None:
+            self.feature_columns = ['remote', 'title', 'stack', 'text', 'experience', 'size']
+        else:
+            self.feature_columns = feature_columns
+        if feature_names_weights is None:
+            self.feature_names_weights = {
+                'remote_similarity': 1,
+                'title_similarity': 0.8,
+                'stack_similarity': 0.8,
+                'text_similarity': 0.7,
+                'experience_similarity': 0.6,
+                'size_similarity': 0.5
+            }
+        else:
+            self.feature_names_weights = feature_names_weights
+        self.feature_names = None
+        self.original_df = self.preprocess()
+
+    def compute_similarity(self):
+        """Returns a Series of similarities for a given job."""
+        res = self.compute_all_similarities(self.original_df, self.feature_columns, self.job_id)
+        df = self.compute_weighted_similarity(res, self.feature_names_weights)
+        return self.normalise_computed_weighted_similarity(df)
+
+    def preprocess(self):
+        df = self.extract_data(self.columns)
+        self.fill_na(df, self.columns)
+        df['stack'] = df.apply(self.strip_stack, axis=1)
+        return df
+
+    def extract_data(self, columns):
+        engine = create_engine(f"postgresql://{USER}:{PWD}@localhost:5432/job_market")
+        query = 'SELECT * FROM relevant;'
+        relevant = pd.read_sql_query(query, engine)
+        relevant = relevant[
+            ['id', 'title', 'company', 'remote', 'location', 'stack', 'education', 'size', 'experience', 'rank', 'url',
+             'industry', 'type', 'created_at', 'text', 'summary']]
+        # print(relevant.info())
+
+        user_df = relevant[['id']]
+        item_df = relevant[columns]
+        df = pd.merge(user_df, item_df, on='id')
+        return df
+
+    def fill_na(self, df, columns):
+        for column in columns:
+            df[column] = df[column].fillna('')
+
+    def strip_stack(self, row):
+        new_row = row['stack'].replace('{', '').replace('}', '').split(',')
+        return new_row
+        # return [w for w in row['stack']] # ast literal eval
+
+    def combine_features(self, row, feature_column):
+        new_row = ''
+        if feature_column == 'stack':  # a list of words
+            # print('list of words\n')
+            for w in row['stack']:
+                new_row = new_row + ' ' + w
+                return new_row
+        elif feature_column == 'title' or feature_column == 'experience' or feature_column == 'size':
+            # print('title\n')
+            return row[feature_column]
+        elif feature_column == 'text':
+            for w in [w for w in row['text'].split(' ')]:
+                new_row = new_row + ' ' + w
+                return new_row
+        elif re.search(' +', row[feature_column]):  # multiple words
+            # print('multiple words\n')
+            for i in range(len(row[feature_column])):
+                new_row = new_row + ' ' + str(row[feature_column[i]])
+            return new_row
+        elif not re.search(' +', row[feature_column]):  # only one word
+            # print(f'one word: {row[feature_column]}\n')
+            return row[feature_column]
+
+    def extract_features(self, df):
+        cv = CountVectorizer()
+        count_matrix = cv.fit_transform(df["combined_features"])
+        # print(count_matrix.shape)
+        return count_matrix
+
+    def compute_individual_similarity(self, df, job_id, feature_column, feature_name):
+        # Combine the features in one field
+        df["combined_features"] = df.apply(lambda x: self.combine_features(x, feature_column), axis=1)
+
+        # Compute the count matrix then similarities
+        count_matrix = self.extract_features(df)
+        cosine_sim = cosine_similarity(count_matrix)
+
+        # Get similar jobs for one job_id
+        similar_jobs = list(enumerate(cosine_sim[job_id]))
+
+        # Keep similarity scores in a Series
+        similarities = [similar_jobs[i][1] for i in range(len(similar_jobs))]
+        return pd.Series(similarities).rename(feature_name)
+
+    def compute_all_similarities(self, df, feature_columns, job_id):
+        # Create base DataFrame indicating job_id that similarity is computed for
+        individual_similarity = self.compute_individual_similarity(df=df, job_id=job_id,
+                                                                   feature_column=self.feature_columns[0],
+                                                                   feature_name='')
+        individual_similarities = pd.DataFrame(index=individual_similarity.index)
+        individual_similarities['job_id'] = job_id
+
+        # Get features names
+        self.feature_names = list()
+
+        # For each feature, compute similarity in its own column
+        for feature_column in feature_columns:
+            feature_name = feature_column + '_similarity'
+            self.feature_names.append(feature_name)
+            individual_similarity = self.compute_individual_similarity(df=df, job_id=job_id,
+                                                                       feature_column=feature_column,
+                                                                       feature_name=feature_name)
+            individual_similarities = individual_similarities.merge(individual_similarity, left_index=True,
+                                                                    right_index=True)
+
+        return df.merge(individual_similarities, left_index=True, right_index=True)
+
+    def compute_weighted_similarity(self, res, feature_names_weights):
+        weights = list(feature_names_weights.values())
+        weighted = res[self.feature_names].apply(lambda x: x * weights, axis=1)
+        res['weighted_similarity'] = weighted.apply(np.sum, axis=1)
+        return res.sort_values(by='weighted_similarity', ascending=False)
+
+    def normalise_computed_weighted_similarity(self, weighted_df):
+        top = (weighted_df['weighted_similarity'] - min(weighted_df['weighted_similarity']))
+        bot = (max(weighted_df['weighted_similarity']) - min(weighted_df['weighted_similarity']))
+        weighted_df[f'similarity_{self.job_id}'] = top / bot
+        return weighted_df[f'similarity_{self.job_id}']
+
+    def compute_mean_similarities(self, df, job_ids):
+        # TODO: calculate mean of similarities of different jobs
+        # print(self.feature_names, '\n')
+        sim_columns = [f'similarity_{job_id}' for job_id in job_ids]
+        df['mean_similarity'] = df[sim_columns].mean(axis=1)
+        return df
+        # print(df[self.feature_names])
 
-    user_df = relevant[['id']]
-    item_df = relevant[['id', 'title', 'company', 'remote', 'stack']]
-    df = pd.merge(user_df, item_df, on='id')
-    return df
-
-
-def fill_na_features(df):
-    features = ['title', 'remote', 'location', 'stack', 'education', 'size', 'experience', 'text']
-    for feature in features:
-        df[feature] = df[feature].fillna('')
-
-
-def strip_stack(row):
-    new_row = row['stack'].replace('{', '').replace('}', '').split(',')
-    return new_row
-
-
-def combine_features(row):
-    new_row = row['title'] + ' ' + row['remote']
-    for w in row['stack_2']:
-        new_row = new_row + ' ' + w
-    return new_row
-
-
-def extract_features(df):
-    cv = CountVectorizer()
-    count_matrix = cv.fit_transform(df["combined_features"])
-    print("Count Matrix:\n", count_matrix.toarray())
-    print("Count Matrix:\n", count_matrix.toarray().shape)
-    return count_matrix
-
-
-def get_index_from_id(df, _id):
-    return df[df.id == _id].index
-
-
-def get_title_from_index(df, index):
-    return df[df.index == index]["title"].values[0]
-
-
-def get_row_from_index(df, index):
-    return df[df.index == index]
-
-
-def find_similar_jobs(df, job_id, cosine_sim):
-    job_index = get_index_from_id(df, job_id)[0]
-    similar_jobs = list(enumerate(cosine_sim[job_index]))
-    sorted_similar_jobs = sorted(similar_jobs, key=lambda x: x[1], reverse=True)
-    similar_jobs = [get_row_from_index(df, job[0]) for job in sorted_similar_jobs]
-    return similar_jobs
+    def get_id_from_index(self, df, index):
+        return df[df.index == index]["id"].values[0]
 
 
 def main():
-    # Prepare data
-    df = extract_data()
-    fill_na_features(df)
-    df['stack_2'] = df.apply(strip_stack, axis=1)
-    df["combined_features"] = df.apply(combine_features, axis=1)
-
-    # Calculate cosine similarity
-    count_matrix = extract_features(df)
-    cosine_sim = cosine_similarity(count_matrix)
-    print(cosine_sim)
-
-    # Define the list of job IDs we like
-    job_ids = [56987, 56988]
-
-    # Find similar jobs
-    i = 0
+    job_ids = [333, 444, 555]
+    base_recommender = Recommender(job_id=job_ids[0])
+    original_df = base_recommender.original_df
     for job_id in job_ids:
-        similar_jobs = find_similar_jobs(df, job_id, cosine_sim)
-        print(f"Similar jobs for Job ID {job_id}:")
-        for job in similar_jobs:
-            print(job)
-            i = i + 1
-            if i > 15:
-                break
+        recommender = Recommender(job_id=job_id)
+        sim = recommender.compute_similarity()  # Adds column similarity
+        original_df = original_df.merge(sim, left_index=True, right_index=True)
+    df = base_recommender.compute_mean_similarities(original_df, job_ids)
+    # df = df.sort_values(by='mean_similarity', ascending=False)  # Will shuffle index
+    print(df)
+    print(df.iloc[333])
+    print(base_recommender.get_id_from_index(df, 333))
 
 
 if __name__ == '__main__':
     main()
```

## data_job_etl/transform/preprocess.py

```diff
@@ -57,7 +57,10 @@
             return 'partiel'
         elif 'ponctuel' in original:
             return 'ponctuel'
         elif 'total' in original:
             return 'total'
         else:
             return original
+
+
+print(dir(Preprocessor))
```

## data_job_etl/update_table.py

```diff
@@ -10,14 +10,15 @@
     """
     Modify table once outside the automated workflow.
     """
 
     def __init__(self):
         self.extractor = Extractor()
         self.loader = Loader()
+        print(dir(Preprocessor))
 
     def extract_processed_jobs(self):
         return self.extractor.extract_table('processed_jobs')
 
     def update_remote(self):
         """Modification of remote field in processed_jobs table."""
         processed_jobs = self.extract_processed_jobs()
```

## Comparing `data_job_etl-1.1.1.dist-info/RECORD` & `data_job_etl-1.1.3.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 data_job_etl/etl.py,sha256=XLATUe1psRm9j3fWYBxL0-jwC7eOOvcIY-B04T2qCCo,1363
 data_job_etl/extract/extract.py,sha256=KZ2Vtye9N6xzLzAOxx-DeljrWobCvLHF4bSqDYtA_Cs,418
 data_job_etl/file.log,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 data_job_etl/load/create_tables.py,sha256=InZHxc-rU0W-1mLmgU9Ul7b5w7CkSI4aoW84tQNx-OU,380
 data_job_etl/load/load.py,sha256=CzogYxoKwlh4TX0sYa1i-oVciMl-q2OWCyPmi0EGG98,4661
 data_job_etl/message.py,sha256=8nHJ7Lrh7IHZ0sPZ5Ge6TNP4pJIheOrJz8F9bxUq4_Y,5979
 data_job_etl/rank.py,sha256=opyH6EnTLpLUs-166yN71uiCu4Yklp4yzGJb5_MiNUI,4480
-data_job_etl/recommendation_system.py,sha256=-TWysP-GoVNrZf1HrA3xLugnmmzbCawMznb0GJelm2U,3040
+data_job_etl/recommendation_system.py,sha256=QvF-hJMHk5dv-4yRhpMO0STcQnhRB3VIqTUO_Uivvw0,8076
 data_job_etl/summarise.py,sha256=-CwLg-gTooiRHwCFBlLytwRuM9T1wqwWCq4P7ZQ9_Ok,2547
 data_job_etl/transform/file.log,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-data_job_etl/transform/preprocess.py,sha256=S8cW6C7z2nBCcOQxxCqF4TEkDg6JpUEXgxf-VW3XHbE,1965
+data_job_etl/transform/preprocess.py,sha256=xzGV7Lg0cWW8hDCZcQbYCiOKvN1O2zSEOKeZzSiKRyc,1991
 data_job_etl/transform/process.py,sha256=xgL0CWAVwJN4kSECexOI4odt7HWWyk90943Uzcv8B7I,2254
-data_job_etl/update_table.py,sha256=9maWu5wjwXFseMbs5B6yfS6_CygBRW7DzJtKzo_jSIA,1641
-data_job_etl-1.1.1.dist-info/METADATA,sha256=iPaF6D09SeYcK_r8ueFqqTTJ9-hq6wQKpYP0M3Gg4Jw,465
-data_job_etl-1.1.1.dist-info/WHEEL,sha256=WGfLGfLX43Ei_YORXSnT54hxFygu34kMpcQdmgmEwCQ,88
-data_job_etl-1.1.1.dist-info/RECORD,,
+data_job_etl/update_table.py,sha256=Hg1zcM3PjgMvxKSkqjb-8Anw50rta9Y43fKg41xri0o,1674
+data_job_etl-1.1.3.dist-info/METADATA,sha256=7glyf6qE7AfiUFGOjghTvHKZzWt6iaoxFaO_hWDxFqA,465
+data_job_etl-1.1.3.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+data_job_etl-1.1.3.dist-info/RECORD,,
```

