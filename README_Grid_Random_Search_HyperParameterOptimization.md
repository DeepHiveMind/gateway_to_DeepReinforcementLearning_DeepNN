| ALGORITHMS  | DEFAULT PARAMETERS | GRID SEARCH AND RANDOM SEARCH PARAMETERS|
| --- | --- |--- | 
|SVC|	clf = SVC(gamma='auto') |[{'kernel': ['rbf'], 'gamma': [1e-3, 1e-4], 'C': [1, 10, 100, 1000]}|
|RandomForestClassifier | clf = RandomForestClassifier(n_estimators=100, max_depth=2,random_state=0) |random_grid = {'n_estimators': n_estimators,'max_features': max_features, 'max_depth': max_depth, 'min_samples_split': min_samples_split,'min_samples_leaf':min_samples_leaf,'bootstrap': bootstrap}|
|RandomForestRegressor|	regr = RandomForestRegressor(max_depth=2, random_state=0, n_estimators=100) |	tuned_parameters = {'n_estimators': [500, 700, 1000], 'max_depth': [None, 1, 2, 3], 'min_samples_split': [1, 2, 3]} |
|LinearRegression	| reg = LinearRegression().fit(X, y) |	parameters = {'fit_intercept':('True', 'False'), 'normalize':('True', 'False'), 'copy_X':('True', 'False')}|
|KMeans |	kmeans = KMeans(n_clusters=2, random_state=0).fit(X) | param_grid = {"n_clusters": range(2, 11)} |
|Hierarchical Clustering	clustering (AgglomerativeClustering) | ac = AgglomerativeClustering().fit(X) |	ac =AgglomerativeClustering(memory='mycachedir',  compute_full_tree=True)|
|association_rules |	from mlxtend.frequent_patterns import association_rules /n rules = association_rules(frequent_itemsets, metric="lift", min_threshold=1) | |
	

