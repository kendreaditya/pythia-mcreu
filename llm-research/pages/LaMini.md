- ## Distilled Notes
	- Current model are resource intensive, and limit the accessibility to many smaller NLP researchers. [(Nityasya et al., 2020)](((645ab572-f74d-488b-907f-2f9e0140bbff))) [(Wu et al., 2023)](((645ab572-9fa0-4269-9bfb-5b54d6f4caca)))
	- Recent research (We et al., 2023):
		- fails to provide compressive evaluations of the resulting models ((645ab572-2ab2-45b2-bcc3-cdf6690d8e6d))
		- train on small-scaled distilled datasets ((645ab572-1693-437b-8f08-1df9c5325cef))
		- train on non-diverse datasets ((645ab572-1693-437b-8f08-1df9c5325cef))
		- lack training on multi-dialogue conversations ((645ab572-2265-468b-b601-8680e9ec1c9e))
	- Furthermore, training large models raises the concern of the environmental impact and energy footprint [(Strubell et al., 2019)](((645ab572-9b01-4c72-b3ba-f861d19114a6))).
	- Tested both encoder-decoder and decoder-only models and found that T5-based models outperformed their decoder-only counter part models and were on-par with models 7x their size. Hence, for smaller models and currently available datasets, encoder-decoder models are shown to have superior performance. (Wu et al., 2023) [1](((645ab572-432c-47dc-9f16-f1657d9d1757))) [2](((645ab572-5e0f-49b6-95aa-9fff47761e47)))
	- [(Wu et al., 2023)](((645ab572-a3fc-4252-905c-c0c46efc8172))) created a large dataset consisting of prompts from self-instruct, Alpaca, P3, FLAN, and created their own GPT guided dataset of 2.58M instructions.
	- LaMini approaches the problem of efficient scaled down models by using knowledge distillation to allow a more concise replication of larger teacher models. ((645ab572-cf54-4130-8ba5-519757963380)) ((645ab572-b20b-48be-8f6f-90e3561013f8))
- ## Literature Notes
	- # [2304.14402](x-devonthink-item://03A9F23C-2542-4E27-BA4A-4F0D6FBCCE96)
	- ## [Page 1](x-devonthink-item://03A9F23C-2542-4E27-BA4A-4F0D6FBCCE96?page=0&annotation=Highlight&x=88&y=534)
	  id:: 645ab572-9fa0-4269-9bfb-5b54d6f4caca
	  * {==However, these models are resource intensive. To alleviate this issue, we explore distilling knowledge from instruction- tuned LLMs to much smaller ones.==}
	  how effective was it and what were the short comings?
	- ## [Page 1](x-devonthink-item://03A9F23C-2542-4E27-BA4A-4F0D6FBCCE96?page=0&annotation=Highlight&x=88&y=498)
	  id:: 645ab572-a3fc-4252-905c-c0c46efc8172
	  * {==large set of 2.58M in- structions based on both existing and newly- generated instructions.==}
	- ## [Page 1](x-devonthink-item://03A9F23C-2542-4E27-BA4A-4F0D6FBCCE96?page=0&annotation=Highlight&x=88&y=473)
	  * {==we design our instructions to cover a broad set of topics to ensure.==}
	  add smart assistent caibalities by using providing model ios APIs for langchain
	- ## [Page 1](x-devonthink-item://03A9F23C-2542-4E27-BA4A-4F0D6FBCCE96?page=0&annotation=Highlight&x=306&y=380)
	  id:: 645ab572-f74d-488b-907f-2f9e0140bbff
	  * {==Moreover, the accessibility of large models is a real concern for many NLP practitioners due to lim- ited access to computing resources \(Nityasya et al., 2020\).==}
	- ## [Page 1](x-devonthink-item://03A9F23C-2542-4E27-BA4A-4F0D6FBCCE96?page=0&annotation=Highlight&x=88&y=390)
	  id:: 645ab572-432c-47dc-9f16-f1657d9d1757
	  * {==both from the encoder-decoder as well as the decoder-only families.==}
	- ## [Page 1](x-devonthink-item://03A9F23C-2542-4E27-BA4A-4F0D6FBCCE96?page=0&annotation=Highlight&x=306&y=177)
	  id:: 645ab572-1693-437b-8f08-1df9c5325cef
	  * {==Specifically, these works often \(i\) provide a small-scale distilled dataset \(ii\) that is not necessarily diverse, and a \(iii\) limited number of models \(typically only one\), \(iv\) with- out comprehensive evaluation nor analysis of the models’ performance.==}
	  need to adress is in my paper
	- ## [Page 1](x-devonthink-item://03A9F23C-2542-4E27-BA4A-4F0D6FBCCE96?page=0&annotation=Highlight&x=71&y=107)
	  id:: 645ab572-9b01-4c72-b3ba-f861d19114a6
	  * {==Consequently, scaling the models raises many issues such as those related to the energy footprint \(Strubell et al., 2019\).==}
	- ## [Page 2](x-devonthink-item://03A9F23C-2542-4E27-BA4A-4F0D6FBCCE96?page=1&annotation=Highlight&x=71&y=428)
	  id:: 645ab572-2ab2-45b2-bcc3-cdf6690d8e6d
	  * {==providing a comprehensive evaluation of the resulting models.==}
	- ## [Page 2](x-devonthink-item://03A9F23C-2542-4E27-BA4A-4F0D6FBCCE96?page=1&annotation=Highlight&x=71&y=360)
	  * {==We assess the performance of the models on various NLP down- stream tasks, in addition to manual human eval- uation of the model’s outputs. This analysis of- fers a more in-depth understanding of the models’ strengths and weaknesses.==}
	- ## [Page 2](x-devonthink-item://03A9F23C-2542-4E27-BA4A-4F0D6FBCCE96?page=1&annotation=Highlight&x=306&y=302)
	  id:: 645ab572-cf54-4130-8ba5-519757963380
	  * {==2.2 Knowledge Distillation==}
	  this is porbally where I can have some impormvemtn
	- ## [Page 2](x-devonthink-item://03A9F23C-2542-4E27-BA4A-4F0D6FBCCE96?page=1&annotation=Highlight&x=93&y=250)
	  * {==is ⇥50 larger than the one released by==}
	- ## [Page 2](x-devonthink-item://03A9F23C-2542-4E27-BA4A-4F0D6FBCCE96?page=1&annotation=Highlight&x=306&y=81)
	  id:: 645ab572-b20b-48be-8f6f-90e3561013f8
	  * {==This approach involves generating a synthetic output by running inference with the teacher model, which is then used to train the student model.==}
	  This is very similar to supervised, and can be used again
	- ## [Page 3](x-devonthink-item://03A9F23C-2542-4E27-BA4A-4F0D6FBCCE96?page=2&annotation=Highlight&x=71&y=378)
	  * {==our work is distinct in that we train our model on a considerably larger dataset and distilled it into much smaller models.==}
	- ## [Page 3](x-devonthink-item://03A9F23C-2542-4E27-BA4A-4F0D6FBCCE96?page=2&annotation=Highlight&x=71&y=81)
	  * {==wo strategies to generate instruc- tions in this section: the example-guided and the topic-guided.==}
	- ## [Page 4](x-devonthink-item://03A9F23C-2542-4E27-BA4A-4F0D6FBCCE96?page=3&annotation=Highlight&x=71&y=237)
	  * {==3.2 Response Generation==}
	  What is fundamentally wrong with the lamini models? Why are they performing worse on accuracy?
	- ## [Page 5](x-devonthink-item://03A9F23C-2542-4E27-BA4A-4F0D6FBCCE96?page=4&annotation=Highlight&x=306&y=205)
	  * {==Another noteworthy obser- vation is that gpt-3.5-turbo is even more prone to generated the responses with factual errors when we provide the topics.==}
	  see research for finetuning with refrences
	- ## [Page 6](x-devonthink-item://03A9F23C-2542-4E27-BA4A-4F0D6FBCCE96?page=5&annotation=Highlight&x=71&y=234)
	  * {==We finetune all models over 5 epochs and a batch size of 1024. For our encoder-decoder models, we use a learning rate of 5 ⇥ 10 4 following Chung et al. \(2022\). For our decoder-only models, we follow the same configu- ration as Alpaca \(Taori et al., 2023\) including the learning rate of 2 ⇥ 10 5. We use HuggingFace’s transformers for training. Moreover, we use the same prompt wrapper as Alpaca \(Taori et al., 2023\), hence we also wrap our instruction similarly during inference.==}
	- ## [Page 7](x-devonthink-item://03A9F23C-2542-4E27-BA4A-4F0D6FBCCE96?page=6&annotation=Highlight&x=86&y=568)
	  * {==T5 LaMini-T5 F-T5 LaMini-F-T5 C-GPT LaMini-C GPT-2 LaMini-GPT LLaMa Alpaca \#params. 738M 783M OpenBookQA 32.8 36.0 31.2 34.0 SciQ 82.4 84.5 93.8 86.7 RACE 31.5 32.6 40.9 32.8 ARC 25.4 29.0 30.7 31.8 PIQA 55.9 67.2 72.2 70.6 ReCoRD 73.1 68.7 76.7 70.4 SST 50.2 90.3 94.0 93.1 MRPC 34.3 71.1 82.6 77.9 RTE 79.8 57.0 87.4 65.0 MultiNLI 61.3 54.7 72.4 61.4 MultiNLI \(mis\) 63.1 55.8 72.0 61.0 WSC 60.4 59.0 66.7 64.1 WinoGrande 55.2 54.9 59.9 56.0 WiC 49.4 50.5 64.7 63.8 HellaSwag 38.9 40.6 48.7 43.7 Average 52.9 56.8 66.3 60.8 1.3B 1.5B 29.0 34.0 32.0 39.8 42.4 73.0 79.4 76.1 80.4 66.3 30.3 32.9 33.1 39.1 39.9 25.3 30.3 28.5 35.8 41.4 66.8 66.9 70.5 71.3 77.5 75.0 66.3 84.4 78.5 91.4 51.3 90.3 49.1 93.5 53.0 68.4 71.3 63.2 76.0 68.4 53.1 65.7 52.3 67.9 53.4 35.2 47.4 36.5 67.5 34.4 35.4 49.2 37.0 69.3 35.6 62.3 57.1 73.3 69.6 80.6 51.9 51.8 58.3 56.0 67.0 50.2 50.2 49.8 52.4 50.0 38.4 38.7 50.9 48.3 73.0 49.7 55.4 53.0 63.0 58.3 7B 43.2 69.6 42.2 41.8 76.0 87.4 85.8 74.3 67.1 38.8 39.6 77.3 65.7 57.5 68.7 62.3==}
	- ## [Page 7](x-devonthink-item://03A9F23C-2542-4E27-BA4A-4F0D6FBCCE96?page=6&annotation=Highlight&x=306&y=184)
	  id:: 645ab572-5e0f-49b6-95aa-9fff47761e47
	  * {==Especially, T5-based models of 200M parameters is competitive against LaMini- GPT-1.5B for human evaluation result. We recom- mend further exploration of the encoder-decoder architecture for language models, given their po- tential, as demonstrated in our experiments.==}
	- ## [Page 8](x-devonthink-item://03A9F23C-2542-4E27-BA4A-4F0D6FBCCE96?page=7&annotation=Highlight&x=71&y=347)
	  * {==There- fore, there may be a correlation between the ini- tial model’s performance and the performance achieved after instruction tuning.==}
	- ## [Page 9](x-devonthink-item://03A9F23C-2542-4E27-BA4A-4F0D6FBCCE96?page=8&annotation=Highlight&x=93&y=225)
	  id:: 645ab572-2265-468b-b601-8680e9ec1c9e
	  * {==Single Turn Dialog: While our training data, as well as our user-oriented evaluation, consist of “dialog-like” instruction, our models are not designed to handle multi-turn dialog.==}
	  combated with open assistens tree of conversations
-