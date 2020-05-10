| ALGORITHMS  | DEFAULT PARAMETERS | GRID SEARCH AND RANDOM SEARCH PARAMETERS|
| --- | --- |--- | 
|SVC|SVC	clf = SVC(gamma='auto') |[{'kernel': ['rbf'], 'gamma': [1e-3, 1e-4], 'C': [1, 10, 100, 1000]}|
|RandomForestClassifier | clf = RandomForestClassifier(n_estimators=100, max_depth=2,...                              random_state=0) |random_grid = {'n_estimators': n_estimators,'max_features': max_features, 'max_depth': max_depth, 'min_samples_split': min_samples_split,'min_samples_leaf':min_samples_leaf,'bootstrap': bootstrap}|
