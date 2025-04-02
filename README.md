# Selection_sort
N=int(input())
arr=list(map(int,input().split()))

for i in range(N-1):
    min_index=i
    for j in range(i+1,N):
        if arr[j]<arr[min_index]:
           min_index=j
    arr[i],arr[min_index]=arr[min_index],arr[i]
    print(*arr)
