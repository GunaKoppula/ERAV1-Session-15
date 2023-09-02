# ERA-SESSION15 Vanilla Transformer Implementation in PytorchLightning

### Achieved:
1. **Training Loss: 2.920**
2. **CER Score: 0.691**
3. **BLEU Score: 0.000**
4. **WER Score: 1.080**

### Tasks:
1. :heavy_check_mark: Rewrite the whole code covered in the class in Pytorch-Lightning
2. :heavy_check_mark: Train the model for 10 epochs
3. :heavy_check_mark: Achieve a loss of less than 4

### Results
![image](https://github.com/GunaKoppula/ERAV1-Session-15/assets/61241928/ac6a527d-cde1-491a-910c-ce2c96c41ff8)
**Note:** Detailed results are presnt in results folder as a CSV file

### Model Summary
```python
   | Name                                    | Type               | Params
--------------------------------------------------------------------------------
0  | transformer                             | Transformer        | 75.1 M
1  | transformer.encoder                     | Encoder            | 18.9 M
2  | transformer.encoder.layers              | ModuleList         | 18.9 M
3  | transformer.encoder.norm                | LayerNormalization | 2     
4  | transformer.decoder                     | Decoder            | 25.2 M
5  | transformer.decoder.layers              | ModuleList         | 25.2 M
6  | transformer.decoder.norm                | LayerNormalization | 2     
7  | transformer.src_embed                   | InputEmbeddings    | 8.0 M 
8  | transformer.src_embed.embedding         | Embedding          | 8.0 M 
9  | transformer.tgt_embed                   | InputEmbeddings    | 11.5 M
10 | transformer.tgt_embed.embedding         | Embedding          | 11.5 M
11 | transformer.src_pos                     | PositionalEncoding | 0     
12 | transformer.src_pos.dropout             | Dropout            | 0     
13 | transformer.tgt_pos                     | PositionalEncoding | 0     
14 | transformer.tgt_pos.dropout             | Dropout            | 0     
15 | transformer.projection_layer            | ProjectionLayer    | 11.5 M
16 | transformer.projection_layer.projection | Linear             | 11.5 M
17 | loss_fn                                 | CrossEntropyLoss   | 0     
18 | cer_metric                              | CharErrorRate      | 0     
19 | wer_metric                              | WordErrorRate      | 0     
20 | bleu_metric                             | BLEUScore          | 0     
--------------------------------------------------------------------------------
75.1 M    Trainable params
0         Non-trainable params
75.1 M    Total params
300.532   Total estimated model params size (MB)
```
### Loss & Other Metrics
**Training Loss:**
![image](https://github.com/GunaKoppula/ERAV1-Session-15/assets/61241928/83d10dd5-0f37-4fbc-9812-d724bf16263c)

**CER, WER & BLEU Score:**
![image](https://github.com/GunaKoppula/ERAV1-Session-15/assets/61241928/61015cd1-7360-4169-83d3-146b8ab5945b)

### Tensorboard Plots 
![image](https://github.com/GunaKoppula/ERAV1-Session-15/assets/61241928/e7ad6505-e33b-4b0b-a0aa-9fc714241aae)
![image](https://github.com/GunaKoppula/ERAV1-Session-15/assets/61241928/5524a37d-6393-4d24-9c82-02200eabf750)
![image](https://github.com/GunaKoppula/ERAV1-Session-15/assets/61241928/18145339-6a45-4896-9929-4a17aa69a789)
![image](https://github.com/GunaKoppula/ERAV1-Session-15/assets/61241928/e98b9f74-afb9-4a76-9dd5-c26472a61deb)
