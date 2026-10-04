# AI-based-rescue-mission
DFS(start, target):
  stack   ← [start]
  visited ← { start }
  while stack is not empty:
    cell ← top of stack
    if cell has an unvisited road neighbour n:
        visited ← visited + { n }
        push n
        if n = target: return stack    # the path
    else:
        pop                            # backtrack
  return NO ROUTE                      # target is cut off
