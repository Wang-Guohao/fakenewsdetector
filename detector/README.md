## Requirments
FNR is built in Python 3.6 using PyTorch 1.8. Please use the following command to install the requirements:

```
pip install -r requirements.txt
```

## How to Run
First, place the data address and configuration into the config file in the data directory, and then follow the train 
and test commands.

### train
To run with Optuna for parameter tuning use this command:

```
python main --data "DATA NAME" --use_optuna "NUMBER OF OPTUNA TRIALS" --batch "BATCH SIZE" --epoch "EPOCHS NUMBER"
```

To run without parameter tuning, adjust your parameters in the config file and then use the below command:
```
python main --data "DATA NAME" --batch "BATCH SIZE" --epoch "EPOCHS NUMBER"
```

### test
In the test step, at first, make sure to have the requested 'checkpoint' file then run the following line:
```
python main --data "DATA NAME" --just_test "REQUESTED TRIAL NUMBER"
```

## Reference
[1] Faeze Ghorbanpour, Maryam Ramezani, MohammadAmin Fazli, Hamid R. Rabiee, FNR: A Similarity and Transformer-Based Approach to Detect Multi-Modal Fake News in Social Media, 2021.

[2] Louis-Philippe Morency and Tadas Baltrušaitis. 2017. Multimodal Machine Learning: Integrating Language, Vision and Speech.

[3] An Image is Worth 16x16 Words: Transformers for Image Recognition at Scale. arXiv:2010.11929 (2021)

[4] www.reddit.com/r/fakehistoryporn  www.reddit.com/r/fakefacts 

[5] Technology blog - Thoroughly understand the Google Bert model, https://www.jianshu.com/p/46cb208d45c3

[6]Nakamura, Kai, Sharon Levy, and William Yang Wang. "r/fakeddit: A new multimodal benchmark dataset for fine-grained fake news detection." arXiv preprint arXiv:1911.03854 (2019).

```

