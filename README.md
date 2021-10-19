# 20211019
# 컴퓨터 프로그래밍2 6주차 문자열

#1 문장에 포함된 단어의 빈도수
def solution(text, word):
  result = 0 
  for sub_text in text.split(" "):
    if sub_text == word:
      result += 1
  return result
  
#2 나의 영어 단어 시험 점수는?
def solution(src_text, ref_text):
  same = 0
  for i in range(len(src_text)):
    if src_text[i] not in ref_text:
      src_text = src_text.replace(src_text[i], " ")
    else:
      same += 1
  if same == 0:
    return -1
  return src_text
  
  #3 너와 나의 암호문


