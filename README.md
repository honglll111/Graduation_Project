# 3주차 진도보고서(정민서)
## 활동 주제
OpenAI key 발급 & 프롬프트 코드 작성(Colab)

## 활동 내용
1. OpenAI key 발급 및 카드 등록

2. 프롬프트 코드 작성(Colab)
   
   OPenAI의 공식 문서를 참고하여 prompt engineering을 위한 코드 작성
   
   https://platform.openai.com/docs/guides/images/introduction

         pip install openai
         pip install --upgrade pip

         import openai
         import urllib.request
         from PIL import Image

         openai.api_key = "OpenAI_Key"
         prompt1 = "Prompt_Content"

         response = openai.Image.create_edit(
         image=open('Original_Picture_Directory', 'rb'),
         mask=open('Masking_Picture_Directory', 'rb'),
         prompt=prompt1,
         n=1,
         size="1024x1024",
         response_format='url'
         )

         image_url = response.data[0]['url']

         urllib.request.urlretrieve(url=image_url, filename="gfg.png")
         img = Image.open("gfg.png")
         img.show()
   

     
## 다음주차 계획
- 프롬프트 엔지니어링
