#adding two sets to get our target number
class Solution:
    def twoSum(self, nums, target):
        number = {}
        for i, num in enumerate(nums):
            complement = target - num
            if complement in number:
                return [number[complement], i]
            number[num] = i
