## Reference 
We take Kai Li "https://github.com/kailigo/cvcZSL" and "https://github.com/mboboGO/DVBE" as reference. 

## Download finetuned data
We release fine-tuned images features of CUB on https://drive.google.com/file/d/1G6ZLwANmGqAApVZp3HymBY6dvHAZvROh/view?usp=sharing.
Please download the features and put into folder ./dataset/finetune/CUB/ .
We will release fine-tuned image features of other dataset in the feature.

目前已知BUG，先前訓練完unseen後，接著要來處理seen的程式碼，發現之前下載的finetuned data居然無法用pickle load進來，
重新下載檔案之後就可以正常訓練seen expert了。


## environment setting:
python version: 3.7.6

## The runing commands are below:
### Training unseen expert.
sh train_unseen.sh
### Training seen expert.
sh train_seen.sh
### Evaluation.
sh test.sh

## License
Apache License 2.0
