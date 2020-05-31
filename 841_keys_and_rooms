class Solution:
    def canVisitAllRooms(self, rooms: List[List[int]]) -> bool:
        length = len(rooms)
        if length == 0:
            return False
        visited = [False]*length
        queue = []
        queue.append(rooms[0])
        visited[0] = True
        
        while queue:
            s = queue.pop(0)
            for i in s:
                if visited[i] == False:
                    queue.append(rooms[i])
                    visited[i] = True
        print(visited)
        for i in visited:
            if i == False:
                return False
        return True
    
# time complexity = |V|+|E|
# space complexity = |V|
