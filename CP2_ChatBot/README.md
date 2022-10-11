# CP2_ChatBot


감정에 따른 사용자 질문에 시스템이 답변을 생성하는 모델. 
***
## Transformer 
[📎 모델 코드 참조](https://github.com/2hg7274/CP2/blob/main/CP2_ChatBot/Model/transformer.ipynb)

<br/>

### 결과
<img width="574" alt="스크린샷 2022-10-11 오후 6 07 59" src="https://user-images.githubusercontent.com/94213374/195048373-06f284f8-3009-49e8-922f-2190e8946009.png">

위의 그림과 같이 답변이 제대로 생성되지 않는 것을 확인할 수 있음. <br/>
-> 감정별 데이터의 양이 많지 않고 대사를 살펴보면 다양한 어휘로 구성되어 있지 않기 때문에 적절하지 않는 답변 생성.  

<br/><br/>

## KoGPT-2
[📎 모델 코드 참조](https://github.com/2hg7274/CP2/blob/main/CP2_ChatBot/Model/KoGPT-2.ipynb)  

<br/>

### 결과
<img width="484" alt="스크린샷 2022-10-11 오후 6 13 25" src="https://user-images.githubusercontent.com/94213374/195049530-8500d9d8-dea8-43ab-91fc-d2b76ed0aaea.png">

위의 그림과 같이 Transformer 모델에 비해 적절한 답변을 생성한 것을 알 수 있음.  
따라서 최종적으로 KoGPT-2 모델 결정.  

각 감정에 따른 5개의 챗봇 모델 생성.
<img width="355" alt="스크린샷 2022-10-11 오후 6 16 02" src="https://user-images.githubusercontent.com/94213374/195050057-0369b516-58a1-41a6-b33e-b64d19ff664b.png">




