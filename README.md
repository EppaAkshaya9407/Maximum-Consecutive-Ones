# Maximum-Consecutive-Ones
nums = list(map(int,input("Enter the array elements (0s and 1s):").split()))
n=len(nums)
c = 0
m = 0
for i in range(n):
    if nums[i]==1:
        c+=1
        m=max(m,c)
    else:
        c=0
print("Maximum consecutive ones:",m)
