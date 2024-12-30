#adding two lists to get our target number
class Solution:
    def twoSum(self, nums, target):
        number = {}
        for i, num in enumerate(nums):
            complement = target - num
            if complement in number:
                return [number[complement], i]
            number[num] = i
nums = input("Enter the numbers").split(" ")
nums = [int(num) for num in nums] 
target = int(input("Enter the target number: "))
solution = Solution()
result = solution.twoSum(nums, target)
print("Output:", result)

