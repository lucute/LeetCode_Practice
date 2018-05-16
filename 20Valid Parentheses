#20. Valid Parentheses

class Solution:
    def isValid(self, s):
        """
        :type s: str
        :rtype: bool
        """
        dic = {
            '(':')',
            '{':'}',
            '[':']'
        }
        result = ['1']
        for p in s:
            if len(s) == 0:
                return True
            elif p in dic:
                result.append(dic[p])
            elif p == result[-1]:
                result.pop()
            else:
                return False
        return len(result) == 1
