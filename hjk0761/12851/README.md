# Info
[숨바꼭질 2](https://boj.kr/12851)

- 난이도: 골드 4
- 분류: 그래프 이론, 그래프 탐색, 너비 우선 탐색

## 💡 풀이 방법 요약

bfs 를 통해 풀 수 있었습니다.

각 점을 그래프의 정점으로 생각한다면 정점 n 에서 정점 k 로 가는 최단 거리를 찾는 문제와 동치입니다.

여기서 그래프의 간선은 각 정점 x에 대해서 x+1, x-1, x*2 로 가는 간선이 존재하고, 각 간선의 길이는 1이라고 생각할 수 있습니다.

단, bfs 를 돌 때 목표 정점에 다다랐을 때에 종료하면 해당 정점으로 가는 모든 경우의 수를 구하지 못하므로 break 대신 continue 를 사용하여 큐 안의 남은 간선들도 모두 순회할 수 있도록 해야 합니다.

## 👀 실패 이유

## 🙂 마무리
