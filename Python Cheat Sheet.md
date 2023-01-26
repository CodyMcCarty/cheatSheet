## list
### methods
- `-abs(num)`
- `arr[::3]` every 3rd element
- `arr[::len(arr)-1]` first and last 
### guard
- `if not arr: return []`  
- `return [pos, neg] if len(arr) else []`
- `return [sum(1 for x in arr if x > 0), sum(x for x in arr if x < 0)]`
- `return [len([i for i in arr if i > 0]),sum([i for i in arr if i < 0])] if arr else []`
### flow
- 
```py
default_grading_scale = {
    90: 'A',
    80: 'B',
    70: 'C',
    60: 'D',
    0: 'F'
}

def get_grade(*s, grading_scale = default_grading_scale):
    avg_score = sum(s) / len(s)
    for score in grading_scale:
        if avg_score >= score:
            return grading_scale[score]
    return 'Not Found' 

def get_grade(s1, s2, s3):
    return {6:'D', 7:'C', 8:'B', 9:'A', 10:'A'}.get((s1 + s2 + s3) / 30, 'F')

def get_grade(*grades):
    mean = sum(grades)/len(grades)
    for score, grade in [(90, 'A'), (80, 'B'), (70, 'C'), (60, 'D'), (0, 'F')]:
        if mean >= score:
            return grade
```
- list comprehension and generators
```py
def positive_sum(arr):
    return sum(x for x in arr if x > 0)
```
