if __name__ == '__main__':
    n = int(raw_input())
    sum1=0.0
    student_marks = {}
    for _ in range(n):
        line = raw_input().split()
        name, scores = line[0], line[1:]
        scores = map(float, scores)
        student_marks[name] = scores
    query_name = raw_input()
for i in student_marks:
    if(query_name in student_marks):
              result=list(map(float,student_marks[query_name]))
              sum1=float(sum(result))             
avg=float(sum1/len(result))
avg="{:.2f}".format(avg)
print(avg)
