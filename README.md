# DFS_in_python

```` Python
 def dfsOfGraph(self, V, adj):
        # code here
        visited = [0] * V # initialized visited array using 0
        result = []
        def dfs(node):  
            if visited[node] == 1: # skip already travel node
                return
            visited[node] = 1
            result.append(node)
            for nei in adj[node]:
                dfs(nei)
        dfs(0) # pass 0 source and call it.
        return result
````
