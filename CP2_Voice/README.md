# CP2_Voice

음성 데이터에서 melspectrogram->db와 MFCC를 통한 감정(`기쁨`, `슬픔`, `당황`, `분노`, `중립`)을 분류하는 모델을 각각 생성 후 **ensemble**

---
# Final Model Result
***model8*** 

|parameters|num|
|:------|:----:|
|size|120|
|pad_size|450|
|repeat_size|2|
|sr|16000|
|epochs|50|
|batch_size|128|
|augmentation|O|

[acc-val graph](https://wandb.ai/2hg/cp2/reports/accuracy-val_accuracy-22-10-03-22-57-16---VmlldzoyNzMzMzA1?accessToken=er82d350o8gs4qwkj5oyplhx3vgf9x3gicnmpsfhol8igytpytedja1lmzxfg1ro)

|fold|mels_model_acc|mfcc_model_acc|ensemble_model_acc|
|:--:|:----:|:----:|:----:|
|1|<span style="color:red">**0.6848**</span>|0.6138|0.7610|
|2|0.6467|<span style="color:red">**0.6971**</span>|0.7714|
|3|0.6795|0.6733|0.7448|
|4|0.6648|0.6057|0.7695|
|5|RAM over|RAM over|RAM over|

***1 fold mels_model, 2 fold mfcc_model 선택***
