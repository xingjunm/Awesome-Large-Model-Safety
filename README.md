<div align="center">
  <img src="assets/logo.png" alt="Safety Logo" />
  <a href="https://www.nowpublishers.com/article/Details/SEC-051" target="_blank"><img src="https://img.shields.io/badge/arXiv-b5212f.svg?logo=arxiv" alt="arXiv"></a>
</div>


## 🚀 About the Survey

This survey provides a systematic review of current safety research on large models, covering **Vision Foundation Models** (VFMs), **Large Language Models** (LLMs), **Vision-Language Pre-training** (VLP) models, **Vision-Language Models** (VLMs), **Diffusion Models** (DMs), and large-model-based **Agents**. 

- We present a **comprehensive taxonomy of safety threats** to the above models. 

- We review **defense strategies** （if available)  proposed for each type of attacks as well as commonly used **datasets and benchmarks**.

- We identify and discuss the **open challenges** in large model safety.

--- 
## 🌴 Missing Papers

We will keep updating this survey. Please complete the following form to submit your paper for citation.  

👉 [Submit Your Paper](https://forms.gle/SkFbVvZYw8r8cJJ17)

We appreciate your contributions and look forward to keeping this survey comprehensive and up to date!

⚠️ Note: We completed a major revision of the paper in August 2025. This version reflects our final planned update, and further substantial revisions may not be possible.

---
The survey have been structured with the following considerations for clarity and readability:

- **Models**. We focus on 6 widely studied model categories, including **VFMs**, **LLMs**, **VLPs**, **VLMs**, **DMs**, and **Agents**, and review the attack and defense methods for each separately. These models represent the most popular large models across various domains.

- **Organization**. For each model category, we classify the reviewed works into attacks and defenses, and identify **10** attack types: **adversarial**, **backdoor**, **poisoning**, **jailbreak**, **prompt injection**, **energy-latency**, **membership inference**, **model extraction**, **data extraction**, and **agent** attacks. When both backdoor and poisoning attacks are present for a model category, we combine them into a single **backdoor & poisoning** category due to their similarities. We review the corresponding defense strategies for each attack type immediately after the attacks.

- **Taxonomy**. For each type of attack or defense, we use a two-level taxonomy: **Category → Subcategory**. The **Category** differentiates attacks and defenses based on the threat model (e.g., white-box, gray-box, black-box) or specific subtasks (e.g., detection, purification, robust training/tuning, and robust inference). The **Subcategory** offers a more detailed classification based on their techniques.

- **Granularity**. To ensure clarity, we simplify the introduction of each reviewed paper, highlighting only its key ideas, objectives, and approaches, while omitting technical details and experimental analyses.


<div align="center">
  <figure>
    <img src="/assets/stats.png" alt="Paper stats" />
    <figcaption>Figure 1: Left: The number of safety research papers published over the past four years. Middle: The distribution of research across
different models. Right: The distribution of research across different types of attacks and defenses. </figcaption>
  </figure>
</div>


---

## 🏈 Survey Methodology

First, we conducted a keyword-based search targeting specific model types and threat types to identify relevant papers. Next, we manually filtered out non-safety-related and non-technical papers. For each remaining paper, we categorized its proposed method or framework by analyzing its settings and attack/defense types, assigning them to appropriate categories and subcategories. We collected **390** technical papers, with their distribution across years, model types, and attack/defense strategies illustrated in the following Figures. As shown, safety research on large models has surged significantly since 2023, following the release of ChatGPT. Among the model types, **LLMs** and **DMs** have garnered the most attention, accounting for over **60%** of the surveyed papers. Regarding attack types, **jailbreak**, **adversarial**, and **backdoor attacks** were the most extensively studied. On the defense side, **jailbreak defenses** received the highest focus, followed by **adversarial defenses**.


<div align="center">
    <figure>
  <img src="/assets/New_Fig.png" alt="trends" />
    <figcaption>Figure 2: Paper statistics overview. </figcaption>
    </figure>
</div>

--- 

## 🌟 Papers

<!-- Chapter 2-->
<details>

<summary><span id="ch2">Vision Foundation Model Safety </span></summary>

##### Attacks and Defense for ViT
- Patch-Fool: Are Vision Transformers Always Robust Against Adversarial Perturbations?  
  - Fu, Yonggan, Zhang, Shunyao, Wu, Shang, Wan, Cheng, **and** Lin, Yingyan  
  - *ICLR*, 2022.

- SlowFormer: Adversarial Attack on Compute and Energy Consumption of Efficient Vision Transformers.  
  - Navaneet, KL, Koohpayegani, Soroush Abbasi, Sleiman, Essam, **and** Pirsiavash, Hamed  
  - *CVPR*, 2024.

- PE-Attack: On the Universal Positional Embedding Vulnerability in Transformer-based Models.  
  - Gao, Shiqi, Chen, Tianyu, He, Mingrui, Xu, Runhua, Zhou, Haoyi, **and** Li, Jianxin  
  - *IEEE Transactions on Information Forensics and Security*, 19, 9359-9373, 2024.

- Give me your attention: Dot-product attention considered harmful for adversarial patch robustness.  
  - Lovisotto, Giulio, Finnie, Nicole, Munoz, Mauricio, Mummadi, Chaithanya Kumar, **and** Metzen, Jan Hendrik  
  - *CVPR*, 2022.

- Towards Understanding and Improving Adversarial Robustness of Vision Transformers.  
  - Jain, Samyak, **and** Dutta, Tanima  
  - *CVPR*, 2024.

- On improving adversarial transferability of vision transformers.  
  - Naseer, Muzammal, Ranasinghe, Kanchana, Khan, Salman, Khan, Fahad Shahbaz, **and** Porikli, Fatih  
  - *arXiv preprint arXiv:2106.04169*, 2021.

- Generating transferable adversarial examples against vision transformers.  
  - Wang, Yuxuan, Wang, Jiakai, Yin, Zixin, Gong, Ruihao, Wang, Jingyi, Liu, Aishan, **and** Liu, Xianglong  
  - *ACM MM*, 2022.

- Towards transferable adversarial attacks on vision transformers.  
  - Wei, Zhipeng, Chen, Jingjing, Goldblum, Micah, Wu, Zuxuan, Goldstein, Tom, **and** Jiang, Yu-Gang  
  - *AAAI*, 2022.

- Boosting adversarial transferability with learnable patch-wise masks.  
  - Wei, Xingxing, **and** Zhao, Shiji  
  - *IEEE Transactions on Multimedia*, 26, 3778-3787, 2023.

- Transferable adversarial attack for both vision transformers and convolutional networks via momentum integrated gradients.  
  - Ma, Wenshuo, Li, Yidong, Jia, Xiaofeng, **and** Xu, Wei  
  - *ICCV*, 2023.

- Transferable adversarial attacks on vision transformers with token gradient regularization.  
  - Zhang, Jianping, Huang, Yizhan, Wu, Weibin, **and** Lyu, Michael R  
  - *CVPR*, 2023.

- Improving the Adversarial Transferability of Vision Transformers with Virtual Dense Connection.  
  - Zhang, Jianping, Huang, Yizhan, Xu, Zhuoer, Wu, Weibin, **and** Lyu, Michael R  
  - *AAAI*, 2024.

- Attacking Transformers with Feature Diversity Adversarial Perturbation.  
  - Gao, Chenxing, Zhou, Hang, Yu, Junqing, Ye, YuTeng, Cai, Jiale, Wang, Junle, **and** Yang, Wei  
  - *AAAI*, 2024.

- Decision-based black-box attack against vision transformers via patch-wise adversarial removal.  
  - Shi, Yucheng, Han, Yahong, Tan, Yu-an, **and** Kuang, Xiaohui  
  - *NeurIPS*, 2022.

- Improving Transferable Targeted Adversarial Attacks with Model Self-Enhancement.  
  - Wu, Han, Ou, Guanyan, Wu, Weibin, **and** Zheng, Zibin  
  - *CVPR*, 2024.

- Improving Transferability of adversarial samples via Critical Region-oriented Feature-level Attack.  
  - Li, Zhiwei, Ren, Min, Jiang, Fangling, Li, Qi, **and** Sun, Zhenan  
  - *IEEE Transactions on Information Forensics and Security*, 19, 6650-6664, 2024.

- Adversarial token attacks on vision transformers.  
  - Joshi, Ameya, Jagatap, Gauri, **and** Hegde, Chinmay  
  - *arXiv preprint arXiv:2110.04337*, 2021.

- Understanding and improving adversarial transferability of vision transformers and convolutional neural networks.  
  - Chen, Zhiyu, Xu, Chi, Lv, Huanhuan, Liu, Shangdong, **and** Ji, Yimu  
  - *Information Sciences*, 648, 119474, 2023.

- Towards transferable adversarial attacks on image and video transformers.  
  - Wei, Zhipeng, Chen, Jingjing, Goldblum, Micah, Wu, Zuxuan, Goldstein, Tom, Jiang, Yu-Gang, **and** Davis, Larry S  
  - *IEEE Transactions on Image Processing*, 32, 6346-6358, 2023.

- Towards efficient adversarial training on vision transformers.  
  - Wu, Boxi, Gu, Jindong, Li, Zhifeng, Cai, Deng, He, Xiaofei, **and** Liu, Wei  
  - *ECCV*, 2022.

- Patch Vestiges in the Adversarial Examples Against Vision Transformer Can Be Leveraged for Adversarial Detection.  
  - Li, Juzheng  
  - *AAAI Workshop*, 2022.

- ViTGuard: Attention-aware Detection against Adversarial Examples for Vision Transformer.  
  - Sun, Shihua, Nwodo, Kenechukwu, Sugrim, Shridatt, Stavrou, Angelos, **and** Wang, Haining  
  - *arXiv preprint arXiv:2409.13828*, 2024.

- Understanding and defending patched-based adversarial attacks for vision transformer.  
  - Liu, Liang, Guo, Yanan, Zhang, Youtao, **and** Yang, Jun  
  - *ICML*, 2023.

- Diffusion Models Demand Contrastive Guidance for Adversarial Purification to Advance.  
  - Bai, Mingyuan, Huang, Wei, Li, Tenghui, Wang, Andong, Gao, Junbin, Caiafa, César Federico, **and** Zhao, Qibin  
  - *ICML*, 2024.

- ADBM: Adversarial diffusion bridge model for reliable adversarial purification.  
  - Li, Xiao, Sun, Wenxuan, Chen, Huanran, Li, Qiongxiu, Liu, Yining, He, Yingzhe, Shi, Jie, **and** Hu, Xiaolin  
  - *arXiv preprint arXiv:2408.00315*, 2024.

- Instant Adversarial Purification with Adversarial Consistency Distillation.  
  - Lei, Chun Tong, Yam, Hon Ming, Guo, Zhongliang, **and** Lau, Chun Pong  
  - *arXiv preprint arXiv:2408.17064*, 2024.

- Are vision transformers robust to patch perturbations?  
  - Gu, Jindong, Tresp, Volker, **and** Qin, Yao  
  - *ECCV*, 2022.

- When adversarial training meets vision transformers: Recipes from training to architecture.  
  - Mo, Yichuan, Wu, Dongxian, Wang, Yifei, Guo, Yiwen, **and** Wang, Yisen  
  - *NeurIPS*, 2022.

- Robustifying token attention for vision transformers.  
  - Guo, Yong, Stutz, David, **and** Schiele, Bernt  
  - *ICCV*, 2023.

- Improving robustness of vision transformers by reducing sensitivity to patch corruptions.  
  - Guo, Yong, Stutz, David, **and** Schiele, Bernt  
  - *CVPR*, 2023.

- Improving Interpretation Faithfulness for Vision Transformers.  
  - Hu, Lijie, Liu, Yixin, Liu, Ninghao, Huai, Mengdi, Sun, Lichao, **and** Wang, Di  
  - *ICML*, 2024.

- Random Entangled Tokens for Adversarially Robust Vision Transformer.  
  - Gong, Huihui, Dong, Minjing, Ma, Siqi, Camtepe, Seyit, Nepal, Surya, **and** Xu, Chang  
  - *CVPR*, 2024.

- Diffusion Models for Adversarial Purification.  
  - Nie, Weili, Guo, Brandon, Huang, Yujia, Xiao, Chaowei, Vahdat, Arash, **and** Anandkumar, Animashree  
  - *ICML*, 2022.

- Purify++: Improving Diffusion-Purification with Advanced Diffusion Models and Control of Randomness.  
  - Zhang, Boya, Luo, Weijian, **and** Zhang, Zhihua  
  - *arXiv preprint arXiv:2310.18762*, 2023.

- DifFilter: Defending Against Adversarial Perturbations With Diffusion Filter.  
  - Chen, Yong, Li, Xuedong, Wang, Xu, Hu, Peng, **and** Peng, Dezhong  
  - *IEEE Transactions on Information Forensics and Security*, 19, 6779-6794, 2024.

- MimicDiffusion: Purifying Adversarial Perturbation via Mimicking Clean Diffusion Model.  
  - Song, Kaiyu, Lai, Hanjiang, Pan, Yan, **and** Yin, Jian  
  - *CVPR*, 2024.

- LightPure: Realtime Adversarial Image Purification for Mobile Devices Using Diffusion Models.  
  - Khalili, Hossein, Park, Seongbin, Li, Vincent, Bright, Brandan, Payani, Ali, Kompella, Ramana Rao, **and** Sehatbakhsh, Nader  
  - *ACM MobiCom*, 2024.

- LoRID: Low-Rank Iterative Diffusion for Adversarial Purification.  
  - Zollicoffer, Geigh, Vu, Minh, Nebgen, Ben, Castorena, Juan, Alexandrov, Boian, **and** Bhattarai, Manish  
  - *arXiv preprint arXiv:2409.08255*, 2024.

- You Are Catching My Attention: Are Vision Transformers Bad Learners under Backdoor Attacks?  
  - Yuan, Zenghui, Zhou, Pan, Zou, Kai, **and** Cheng, Yu  
  - *CVPR*, 2023.

- Trojvit: Trojan insertion in vision transformers.  
  - Zheng, Mengxin, Lou, Qian, **and** Jiang, Lei  
  - *CVPR*, 2023.

- Not all prompts are secure: A switchable backdoor attack against pre-trained vision transfomers.  
  - Yang, Sheng, Bai, Jiawang, Gao, Kuofeng, Yang, Yong, Li, Yiming, **and** Xia, Shu-Tao  
  - *CVPR*, 2024.

- DBIA: Data-Free Backdoor Attack Against Transformer Networks.  
  - Lv, Peizhuo, Ma, Hualong, Zhou, Jiachen, Liang, Ruigang, Chen, Kai, Zhang, Shengzhi, **and** Yang, Yunfei  
  - *ICME*, 2023.

- Multi-Trigger Backdoor Attacks: More Triggers, More Threats.  
  - Li, Yige, Ma, Xingjun, He, Jiabo, Huang, Hanxun, **and** Jiang, Yu-Gang  
  - *arXiv preprint arXiv:2401.15295*, 2024.
 
- Defending backdoor attacks on vision transformer via patch processing.  
  - Doan, Khoa D, Lao, Yingjie, Yang, Peng, **and** Li, Ping  
  - *AAAI*, 2023.

- A Closer Look at Robustness of Vision Transformers to Backdoor Attacks.  
  - Subramanya, Akshayvarun, Koohpayegani, Soroush Abbasi, Saha, Aniruddha, Tejankar, Ajinkya, **and** Pirsiavash, Hamed  
  - *WACV*, 2024.

- Backdoor attacks on vision transformers.  
  - Subramanya, Akshayvarun, Saha, Aniruddha, Koohpayegani, Soroush Abbasi, Tejankar, Ajinkya, **and** Pirsiavash, Hamed  
  - *arXiv preprint arXiv:2206.08477*, 2022.


##### Attacks and Defense for SAM

- Practical Region-level Attack against Segment Anything Models.  
  - Shen, Yifan, Li, Zhengyuan, **and** Wang, Gang  
  - *CVPR*, 2024.

- Segment (Almost) Nothing: Prompt-Agnostic Adversarial Attacks on Segmentation Models.  
  - Croce, Francesco, **and** Hein, Matthias  
  - *SaTML*, 2024.

- Attack-SAM: Towards Evaluating Adversarial Robustness of Segment Anything Model.  
  - Zhang, Chenshuang, Zhang, Chaoning, Kang, Taegoo, Kim, Donghun, Bae, Sung-Ho, **and** Kweon, In So  
  - *arXiv preprint arXiv:2305.00866*, 2023.

- Black-box Targeted Adversarial Attack on Segment Anything (SAM).  
  - Zheng, Sheng, **and** Zhang, Chaoning  
  - *arXiv preprint arXiv:2310.10010*, 2023.

- Unsegment Anything by Simulating Deformation.  
  - Lu, Jiahao, Yang, Xingyi, **and** Wang, Xinchao  
  - *CVPR*, 2024.

- Transferable Adversarial Attacks on SAM and Its Downstream Models.  
  - Xia, Song, Yang, Wenhan, Yu, Yi, Lin, Xun, Ding, Henghui, Duan, Lingyu, **and** Jiang, Xudong  
  - *NeurIPS*, 2024.

- Segment Anything Meets Universal Adversarial Perturbation.  
  - Han, Dongshen, Zheng, Sheng, **and** Zhang, Chaoning  
  - *arXiv preprint arXiv:2310.12431*, 2023.

- DarkSAM: Fooling Segment Anything Model to Segment Nothing.  
  - Zhou, Ziqi, Song, Yufei, Li, Minghui, Hu, Shengshan, Wang, Xianlong, Zhang, Leo Yu, Yao, Dezhong, **and** Jin, Hai  
  - *NeurIPS*, 2024.

- ASAM: Boosting Segment Anything Model with Adversarial Tuning.  
  - Li, Bo, Xiao, Haoke, **and** Tang, Lv  
  - *CVPR*, 2024.

- BadSAM: Exploring Security Vulnerabilities of SAM via Backdoor Attacks (Student Abstract).  
  - Guan, Zihan, Hu, Mengxuan, Zhou, Zhongliang, Zhang, Jielu, Li, Sheng, **and** Liu, Ninghao  
  - *AAAI*, 2024.

- UnSeg: One Universal Unlearnable Example Generator is Enough against All Image Segmentation.  
  - Sun, Ye, Zhang, Hao, Zhang, Tiehua, Ma, Xingjun, **and** Jiang, Yu-Gang  
  - *NeurIPS*, 2024.


</details>


<!-- Chapter 3-->
<details>

<summary><span id="ch3">Large Language Model Safety</summary>

##### Adversarial Attack


- Bad Characters: Imperceptible NLP Attacks.  
  - Boucher, Nicholas, Shumailov, Ilia, Anderson, Ross, **and** Papernot, Nicolas  
  - *IEEE S&P*, 2022.

- Is BERT Really Robust? A Strong Baseline for Natural Language Attack on Text Classification and Entailment.  
  - Jin, Di, Jin, Zhijing, Zhou, Joey Tianyi, **and** Szolovits, Peter  
  - *AAAI*, 2020.

- BERT-ATTACK: Adversarial Attack Against BERT Using BERT.  
  - Li, Linyang, Ma, Ruotian, Guo, Qipeng, Xue, Xiangyang, **and** Qiu, Xipeng  
  - *EMNLP*, 2020.

- Gradient-Based Adversarial Attacks Against Text Transformers.  
  - Guo, Chuan, Sablayrolles, Alexandre, Jégou, Hervé, **and** Kiela, Douwe  
  - *EMNLP*, 2021.

- Breaking BERT: Understanding Its Vulnerabilities for Named Entity Recognition Through Adversarial Attack.  
  - Dirkson, Anne, Verberne, Suzan, **and** Kraaij, Wessel  
  - *arXiv preprint arXiv:2109.11308*, 2021.

- Gradient-Based Word Substitution for Obstinate Adversarial Examples Generation in Language Models.  
  - Wang, Y, Shi, P, **and** Zhang, H  
  - *arXiv preprint arXiv:2307.12507*, 2023.

- Expanding Scope: Adapting English Adversarial Attacks to Chinese.  
  - Liu, Hanyu, Cai, Chengyuan, **and** Qi, Yanjun  
  - *TrustNLP*, 2023.

- Adversarial Demonstration Attacks on Large Language Models.  
  - Wang, Jiongxiao, Liu, Zichen, Park, Keun Hee, Jiang, Zhuojun, Zheng, Zhaoheng, Wu, Zhuofeng, Chen, Muhao, **and** Xiao, Chaowei  
  - *arXiv preprint arXiv:2305.14950*, 2023.

- Adversarial Attacks on Large Language Model-Based Systems and Mitigating Strategies: A Case Study on ChatGPT.  
  - Liu, Bowen, Xiao, Boao, Jiang, Xutong, Cen, Siyuan, He, Xin, **and** Dou, Wanchun  
  - *Security and Communication Networks*, 2023.

- Adversarial Attacks on Tables with Entity Swap.  
  - Koleva, Aneta, Ringsquandl, Martin, **and** Tresp, Volker  
  - *arXiv preprint arXiv:2309.08650*, 2023.


##### Adversarial Defense

- Baseline Defenses for Adversarial Attacks Against Aligned Language Models.  
  - Jain, Neel, Schwarzschild, Avi, Wen, Yuxin, Somepalli, Gowthami, Kirchenbauer, John, Chiang, Ping-yeh, Goldblum, Micah, Saha, Aniruddha, Geiping, Jonas, **and** Goldstein, Tom  
  - *arXiv preprint arXiv:2309.00614*, 2023.

- Certifying LLM Safety Against Adversarial Prompting.  
  - Kumar, Aounon, Agarwal, Chirag, Srinivas, Suraj, Feizi, Soheil, **and** Lakkaraju, Hima  
  - *arXiv preprint arXiv:2309.02705*, 2023.

- Improving Alignment and Robustness with Circuit Breakers.  
  - Zou, Andy, Phan, Long, Wang, Justin, Duenas, Derek, Lin, Maxwell, Andriushchenko, Maksym, Kolter, J Zico, Fredrikson, Matt, **and** Hendrycks, Dan  
  - *NeurIPS*, 2024.


##### Jailbreak Attack

- Low-Resource Languages Jailbreak GPT-4.  
  - Yong, Zheng-Xin, Menghini, Cristina, **and** Bach, Stephen H  
  - *NeurIPS Workshop*, 2023.

- GPT-4 is Too Smart to be Safe: Stealthy Chat with LLMs via Cipher.  
  - Yuan, Youliang, Jiao, Wenxiang, Wang, Wenxuan, Huang, Jen-tse, He, Pinjia, Shi, Shuming, **and** Tu, Zhaopeng  
  - *arXiv preprint arXiv:2308.06463*, 2023.

- Jailbroken: How Does LLM Safety Training Fail?  
  - Wei, Alexander, Haghtalab, Nika, **and** Steinhardt, Jacob  
  - *NeurIPS*, 2024.

- A Cross-Language Investigation into Jailbreak Attacks in Large Language Models.  
  - Li, Jie, Liu, Yi, Liu, Chongyang, Shi, Ling, Ren, Xiaoning, Zheng, Yaowen, Liu, Yang, **and** Xue, Yinxing  
  - *arXiv preprint arXiv:2401.16765*, 2024.

- EasyJailbreak: A Unified Framework for Jailbreaking Large Language Models.  
  - Zhou, Weikang, Wang, Xiao, Xiong, Limao, Xia, Han, Gu, Yingshuang, Chai, Mingxu, Zhu, Fukang, Huang, Caishuang, Dou, Shihan, Xi, Zhiheng, **and others**  
  - *arXiv preprint arXiv:2403.12171*, 2024.

- Is the System Message Really Important to Jailbreaks in Large Language Models?  
  - Zou, Xiaotian, Chen, Yongkang, **and** Li, Ke  
  - *arXiv preprint arXiv:2402.14857*, 2024.

- TASTLE: Distract Large Language Models for Automatic Jailbreak Attack.  
  - Xiao, Zeguan, Yang, Yan, Chen, Guanhua, **and** Chen, Yun  
  - *EMNLP*, 2024.

- StructuralSleight: Automated Jailbreak Attacks on Large Language Models Utilizing Uncommon Text-Encoded Structure.  
  - Li, Bangxin, Xing, Hengrui, Huang, Chao, Qian, Jin, Xiao, Huangqing, Feng, Linfeng, **and** Tian, Cong  
  - *arXiv preprint arXiv:2406.08754*, 2024.

- CodeChameleon: Personalized Encryption Framework for Jailbreaking Large Language Models.  
  - Lv, Huijie, Wang, Xiao, Zhang, Yuansen, Huang, Caishuang, Dou, Shihan, Ye, Junjie, Gui, Tao, Zhang, Qi, **and** Huang, Xuanjing  
  - *arXiv preprint arXiv:2402.16717*, 2024.

- Play Guessing Game with LLM: Indirect Jailbreak Attack with Implicit Clues.  
  - Chang, Zhiyuan, Li, Mingyang, Liu, Yi, Wang, Junjie, Wang, Qing, **and** Liu, Yang  
  - *ACL*, 2024.

- AutoDAN: Generating Stealthy Jailbreak Prompts on Aligned Large Language Models.  
  - Liu, Xiaogeng, Xu, Nan, Chen, Muhao, **and** Xiao, Chaowei  
  - *ICLR*, 2024.

- GPTFuzzer: Red Teaming Large Language Models with Auto-Generated Jailbreak Prompts.  
  - Yu, Jiahao, Lin, Xingwei, Yu, Zheng, **and** Xing, Xinyu  
  - *arXiv preprint arXiv:2309.10253*, 2023.

- Jailbreaking Black Box Large Language Models in Twenty Queries.  
  - Chao, Patrick, Robey, Alexander, Dobriban, Edgar, Hassani, Hamed, Pappas, George J, **and** Wong, Eric  
  - *NeurIPS Workshop*, 2023.

- MasterKey: Automated Jailbreaking of Large Language Model Chatbots.  
  - Deng, Gelei, Liu, Yi, Li, Yuekang, Wang, Kailong, Zhang, Ying, Li, Zefeng, Wang, Haoyu, Zhang, Tianwei, **and** Liu, Yang  
  - *NDSS*, 2024.

- Enhancing Jailbreak Attack Against Large Language Models through Silent Tokens.  
  - Yu, Jiahao, Luo, Haozheng, Yao-Chieh, Jerry, Guo, Wenbo, Liu, Han, **and** Xing, Xinyu  
  - *arXiv preprint arXiv:2405.20653*, 2024.

- FuzzLLM: A Novel and Universal Fuzzing Framework for Proactively Discovering Jailbreak Vulnerabilities in Large Language Models.  
  - Yao, Dongyu, Zhang, Jianshu, Harris, Ian G, **and** Carlsson, Marcel  
  - *ICASSP*, 2024.

- EnJa: Ensemble Jailbreak on Large Language Models.  
  - Zhang, Jiahao, Wang, Zilong, Wang, Ruofan, Ma, Xingjun, **and** Jiang, Yu-Gang  
  - *arXiv preprint arXiv:2408.03603*, 2024.

- Red Teaming Language Models with Language Models.  
  - Perez, Ethan, Huang, Saffron, Song, Francis, Cai, Trevor, Ring, Roman, Aslanides, John, Glaese, Amelia, McAleese, Nat, **and** Irving, Geoffrey  
  - *EMNLP*, 2022.

- Curiosity-Driven Red-Teaming for Large Language Models.  
  - Hong, Zhang-Wei, Shenfeld, Idan, Wang, Tsun-Hsuan, Chuang, Yung-Sung, Pareja, Aldo, Glass, James, Srivastava, Akash, **and** Agrawal, Pulkit  
  - *ICLR*, 2024.

- “Do Anything Now”: Characterizing and Evaluating In-The-Wild Jailbreak Prompts on Large Language Models.  
  - Shen, Xinyue, Chen, Zeyuan, Backes, Michael, Shen, Yun, **and** Zhang, Yang  
  - *ACM CCS*, 2024.

- Universal and Transferable Adversarial Attacks on Aligned Language Models.  
  - Zou, Andy, Wang, Zifan, Carlini, Nicholas, Nasr, Milad, Kolter, J Zico, **and** Fredrikson, Matt  
  - *arXiv preprint arXiv:2307.15043*, 2023.

- Improved Techniques for Optimization-Based Jailbreaking on Large Language Models.  
  - Jia, Xiaojun, Pang, Tianyu, Du, Chao, Huang, Yihao, Gu, Jindong, Liu, Yang, Cao, Xiaochun, **and** Lin, Min  
  - *arXiv preprint arXiv:2405.21018*, 2024.

- Improved Few-Shot Jailbreaking Can Circumvent Aligned Language Models and Their Defenses.  
  - Zheng, Xiaosen, Pang, Tianyu, Du, Chao, Liu, Qian, Jiang, Jing, **and** Lin, Min  
  - *arXiv preprint arXiv:2406.01288*, 2024.

- Weak-to-Strong Jailbreaking on Large Language Models.  
  - Zhao, Xuandong, Yang, Xianjun, Pang, Tianyu, Du, Chao, Li, Lei, Wang, Yu-Xiang, **and** Wang, William Yang  
  - *arXiv preprint arXiv:2401.17256*, 2024.

- Unlocking Adversarial Suffix Optimization Without Affirmative Phrases: Efficient Black-box Jailbreaking via LLM as Optimizer.  
  - Jiang, Weipeng, Wang, Zhenting, Zhai, Juan, Ma, Shiqing, Zhao, Zhengyu, **and** Shen, Chao  
  - *arXiv preprint arXiv:2408.11313*, 2024.



##### Jailbreak Defense


- SmoothLLM: Defending Large Language Models Against Jailbreaking Attacks. 
  - Robey, Alexander, Wong, Eric, **and** Hassani, Hamed, Pappas, George J  
  - *arXiv preprint arXiv:2310.03684*, 2023.

- Defending Large Language Models Against Jailbreak Attacks via Semantic Smoothing. 
  - Ji, Jiabao, Hou, Bairu, Robey, Alexander, Pappas, George J, Hassani, Hamed, Zhang, Yang, Wong, Eric, **and** Chang, Shiyu  
  - *arXiv preprint arXiv:2402.16192*, 2024.

- SelfDefend: LLMs Can Defend Themselves Against Jailbreaking in a Practical Manner.
  - Wang, Xunguang, Wu, Daoyuan, Ji, Zhenlan, Li, Zongjie, Ma, Pingchuan, Wang, Shuai, Li, Yingjiu, Liu, Yang, Liu, Ning, **and** Rahmel, Juergen  
  - *arXiv preprint arXiv:2406.05498*, 2024.

- Protecting Your LLMs with Information Bottleneck.  
  - Liu, Zichuan, Wang, Zefan, Xu, Linjie, Wang, Jinyu, Song, Lei, Wang, Tianchun, Chen, Chunlin, Cheng, Wei, **and** Bian, Jiang  
  - *NeurIPS*, 2024.

- Defending LLMs Against Jailbreaking Attacks via Backtranslation.
  - Wang, Yihan, Shi, Zhouxing, Bai, Andrew, **and** Hsieh, Cho-Jui  
  - *ACL*, 2024.

- Robust Safety Classifier Against Jailbreaking Attacks: Adversarial Prompt Shield.
  - Kim, Jinhwa, Derakhshan, Ali, **and** Harris, Ian G  
  - *WOAH*, 2024.

- Defensive Prompt Patch: A Robust and Interpretable Defense of LLMs Against Jailbreak Attacks.
  - Xiong, Chen, Qi, Xiangyu, Chen, Pin-Yu, **and** Ho, Tsung-Yi  
  - *arXiv preprint arXiv:2405.20099*, 2024.

- Gradient Cuff: Detecting Jailbreak Attacks on Large Language Models by Exploring Refusal Loss Landscapes.
  - Hu, Xiaomeng, Chen, Pin-Yu, **and** Ho, Tsung-Yi  
  - *NeurIPS*, 2024.

- Jailbreaker in Jail: Moving Target Defense for Large Language Models.
  - Chen, Bocheng, Paliwal, Advait, **and** Yan, Qiben  
  - *MTD*, 2023.

- PARDEN, Can You Repeat That? Defending Against Jailbreaks via Repetition.  
  - Zhang, Ziyang, Zhang, Qizhen, **and** Foerster, Jakob  
  - *arXiv preprint arXiv:2405.07932*, 2024.

- AutoJailbreak: Exploring Jailbreak Attacks and Defenses Through a Dependency Lens.
  - Lu, Lin, Yan, Hai, Yuan, Zenghui, Shi, Jiawen, Wei, Wenqi, Chen, Pin-Yu, **and** Zhou, Pan  
  - *arXiv preprint arXiv:2406.03805*, 2024.

- MoGU: A Framework for Enhancing Safety of LLMs While Preserving Their Usability.
  - Du, Yanrui, Zhao, Sendong, Zhao, Danyang, Ma, Ming, Chen, Yuhan, Huo, Liangyu, Yang, Qing, Xu, Dongliang, **and** Qin, Bing  
  - *NeurIPS*, 2024.


##### Prompt Injection Attacks


- Ignore Previous Prompt: Attack Techniques for Language Models.
  - Perez, Fábio, **and** Ribeiro, Ian  
  - *NeurIPS Workshop*, 2022.

- Prompt Injection Attack Against LLM-integrated Applications. 
  - Liu, Yi, Deng, Gelei, Li, Yuekang, Wang, Kailong, Wang, Zihao, Wang, Xiaofeng, Zhang, Tianwei, Liu, Yepang, Wang, Haoyu, **and others**  
  - *arXiv preprint arXiv:2306.05499*, 2023.

- Not What You've Signed Up For: Compromising Real-World LLM-integrated Applications with Indirect Prompt Injection.
  - Greshake, Kai, Abdelnabi, Sahar, Mishra, Shailesh, Endres, Christoph, Holz, Thorsten, **and** Fritz, Mario  
  - *AISec*, 2023.

- Attack Prompt Generation for Red Teaming and Defending Large Language Models.  
  - Deng, Boyi, Wang, Wenjie, Feng, Fuli, Deng, Yang, Wang, Qifan, **and** He, Xiangnan  
  - *EMNLP*, 2023.

- Formalizing and Benchmarking Prompt Injection Attacks and Defenses.  
  - Liu, Yupei, Jia, Yuqi, Geng, Runpeng, Jia, Jinyuan, **and** Gong, Neil Zhenqiang  
  - *USENIX Security*, 2024.

- Are We There Yet? Revealing the Risks of Utilizing Large Language Models in Scholarly Peer Review.  
  - Ye, Rui, Pang, Xianghe, Chai, Jingyi, Chen, Jiaao, Yin, Zhenfei, Xiang, Zhen, Dong, Xiaowen, Shao, Jing, **and** Chen, Siheng  
  - *arXiv preprint arXiv:2412.01708*, 2024.

- Automatic and Universal Prompt Injection Attacks Against Large Language Models.  
  - Liu, Xiaogeng, Yu, Zhiyuan, Zhang, Yizhe, Zhang, Ning, **and** Xiao, Chaowei  
  - *arXiv preprint arXiv:2403.04957*, 2024.

- Goal-Guided Generative Prompt Injection Attack on Large Language Models.  
  - Zhang, Chong, Jin, Mingyu, Yu, Qinkai, Liu, Chengzhi, Xue, Haochen, **and** Jin, Xiaobo  
  - *arXiv preprint arXiv:2404.07234*, 2024.

- Pleak: Prompt Leaking Attacks Against Large Language Model Applications.  
  - Hui, Bo, Yuan, Haolin, Gong, Neil, Burlina, Philippe, **and** Cao, Yinzhi  
  - *ACM SIGSAC CCS*, 2024.

- Optimization-Based Prompt Injection Attack to LLM-as-a-Judge.  
  - Shi, Jiawen, Yuan, Zenghui, Liu, Yinuo, Huang, Yue, Zhou, Pan, Sun, Lichao, **and** Gong, Neil Zhenqiang  
  - *ACM SIGSAC CCS*, 2024.

- Making LLMs Vulnerable to Prompt Injection via Poisoning Alignment.  
  - Shao, Zedian, Liu, Hongbin, Mu, Jaden, **and** Gong, Neil Zhenqiang  
  - *arXiv preprint arXiv:2410.14827*, 2024.

##### Prompt Injection Defenses

- StruQ: Defending Against Prompt Injection with Structured Queries. 
  - Chen, Sizhe, Piet, Julien, Sitawarin, Chawin, **and** Wagner, David  
  - *USENIX Security*, 2025.

- SPML: A DSL for Defending Language Models Against Prompt Attacks.
  - Sharma, Reshabh K, Gupta, Vinayak, **and** Grossman, Dan  
  - *arXiv preprint arXiv:2402.11755*, 2024.

- Jatmo: Prompt Injection Defense by Task-Specific Finetuning.  
  - Piet, Julien, Alrashed, Maha, Sitawarin, Chawin, Chen, Sizhe, Wei, Zeming, Sun, Elizabeth, Alomair, Basel, **and** Wagner, David  
  - *arXiv preprint arXiv:2312.17673*, 2023.

- Benchmarking and Defending Against Indirect Prompt Injection Attacks on Large Language Models.  
  - Yi, Jingwei, Xie, Yueqi, Zhu, Bin, Kiciman, Emre, Sun, Guangzhong, Xie, Xing, **and** Wu, Fangzhao  
  - *arXiv preprint arXiv:2312.14197*, 2023.

- SecAlign: Defending Against Prompt Injection with Preference Optimization.  
  - Chen, Sizhe, Zharmagambetov, Arman, Mahloujifar, Saeed, Chaudhuri, Kamalika, Wagner, David, **and** Guo, Chuan  
  - *arXiv preprint arXiv:2410.05451v2*, 2025.

##### Backdoor Attacks

- BadPrompt: Backdoor Attacks on Continuous Prompts.  
  - Cai, Xiangrui, Xu, Haidong, Xu, Sihan, Zhang, Ying, *et al.*  
  - *NeurIPS*, 2022.

- BITE: Textual Backdoor Attacks with Iterative Trigger Injection.  
  - Yan, Jun, Gupta, Vansh, **and** Ren, Xiang  
  - *ACL*, 2023.

- PoisonPrompt: Backdoor Attack on Prompt-Based Large Language Models.  
  - Yao, Hongwei, Lou, Jian, **and** Qin, Zhan  
  - *ICASSP*, 2024.

- Prompt as Triggers for Backdoor Attack: Examining the Vulnerability in Language Models.  
  - Zhao, Shuai, Wen, Jinming, Tuan, Luu Anh, Zhao, Junbo, **and** Fu, Jie  
  - *EMNLP*, 2023.

- Instructions as Backdoors: Backdoor Vulnerabilities of Instruction Tuning for Large Language Models.  
  - Xu, Jiashu, Ma, Mingyu Derek, Wang, Fei, Xiao, Chaowei, **and** Chen, Muhao  
  - *NAACL*, 2024.

- Backdoor Attacks for In-Context Learning with Language Models.  
  - Kandpal, Nikhil, Jagielski, Matthew, Tramèr, Florian, **and** Carlini, Nicholas  
  - *ICML Workshop*, 2023.

- BadChain: Backdoor Chain-of-Thought Prompting for Large Language Models.  
  - Xiang, Zhen, Jiang, Fengqing, Xiong, Zidi, Ramasubramanian, Bhaskar, Poovendran, Radha, **and** Li, Bo  
  - *NeurIPS Workshop*, 2024.

- Universal Vulnerabilities in Large Language Models: Backdoor Attacks for In-Context Learning.  
  - Zhao, Shuai, Jia, Meihuizi, Tuan, Luu Anh, Pan, Fengjun, **and** Wen, Jinming  
  - *EMNLP*, 2024.

- Learning to Poison Large Language Models During Instruction Tuning.  
  - Qiang, Yao, Zhou, Xiangyu, Zade, Saleh Zare, Roshani, Mohammad Amin, Zytko, Douglas, **and** Zhu, Dongxiao  
  - *arXiv preprint arXiv:2402.13459*, 2024.

- Is Poisoning a Real Threat to LLM Alignment? Maybe More So Than You Think.  
  - Pathmanathan, Pankayaraj, Chakraborty, Souradip, Liu, Xiangyu, Liang, Yongyuan, **and** Huang, Furong  
  - *ICML Workshop*, 2024.

- Sleeper Agents: Training Deceptive LLMs That Persist Through Safety Training.  
  - Hubinger, Evan, Denison, Carson, Mu, Jesse, Lambert, Mike, Tong, Meg, MacDiarmid, Monte, Lanham, Tamera, Ziegler, Daniel M, Maxwell, Tim, Cheng, Newton, *et al.*  
  - *arXiv preprint arXiv:2401.05566*, 2024.

- Data Poisoning for In-Context Learning.  
  - He, Pengfei, Xu, Han, Xing, Yue, Liu, Hui, Yamada, Makoto, **and** Tang, Jiliang  
  - *arXiv preprint arXiv:2402.02160*, 2024.

- Human-Imperceptible Retrieval Poisoning Attacks in LLM-Powered Applications.  
  - Zhang, Quan, Zeng, Binqi, Zhou, Chijin, Go, Gwihwan, Shi, Heyuan, **and** Jiang, Yu  
  - *arXiv preprint arXiv:2404.17196*, 2024.

- An LLM-Assisted Easy-to-Trigger Poisoning Attack on Code Completion Models: Injecting Disguised Vulnerabilities Against Strong Detection.  
  - Yan, Shenao, Wang, Shen, Duan, Yue, Hong, Hanbin, Lee, Kiho, Kim, Doowon, **and** Hong, Yuan  
  - *USENIX Security*, 2024.

- Composite Backdoor Attacks Against Large Language Models.  
  - Huang, Hai, Zhao, Zhengyu, Backes, Michael, Shen, Yun, **and** Zhang, Yang  
  - *NAACL*, 2024.

- A Gradient Control Method for Backdoor Attacks on Parameter-Efficient Tuning.  
  - Gu, Naibin, Fu, Peng, Liu, Xiyu, Liu, Zhengxiao, Lin, Zheng, **and** Wang, Weiping  
  - *ACL*, 2023.

- TrojLLM: A Black-Box Trojan Prompt Attack on Large Language Models.  
  - Xue, Jiaqi, Zheng, Mengxin, Hua, Ting, Shen, Yilin, Liu, Yepeng, Bölöni, Ladislau, **and** Lou, Qian  
  - *NeurIPS*, 2024.

- Backdooring Instruction-Tuned Large Language Models with Virtual Prompt Injection.  
  - Yan, Jun, Yadav, Vikas, Li, Shiyang, Chen, Lichang, Tang, Zheng, Wang, Hai, Srinivasan, Vijay, **and** Ren, Xiang, Jin, Hongxia  
  - *NAACL*, 2024.

- Uncertainty Is Fragile: Manipulating Uncertainty in Large Language Models.  
  - Zeng, Qingcheng, Jin, Mingyu, Yu, Qinkai, Wang, Zhenting, Hua, Wenyue, Zhou, Zihao, Sun, Guangyan, Meng, Yanda, Ma, Shiqing, Wang, Qifan, *et al.*  
  - *arXiv preprint arXiv:2407.11282*, 2024.

- BadEdit: Backdooring Large Language Models by Model Editing.  
  - Li, Yanzhou, Li, Tianlin, Chen, Kangjie, Zhang, Jian, Liu, Shangqing, Wang, Wenhan, Zhang, Tianwei, **and** Liu, Yang  
  - *ICLR*, 2024.


##### Backdoor Defenses

- IMBERT: Making BERT Immune to Insertion-Based Backdoor Attacks.  
  - He, Xuanli, Wang, Jun, Rubinstein, Benjamin, **and** Cohn, Trevor  
  - *TrustNLP*, 2023.

- Defending Against Insertion-Based Textual Backdoor Attacks via Attribution.  
  - Li, Jiazhao, Wu, Zhuofeng, Ping, Wei, Xiao, Chaowei, **and** Vydiswaran, VG  
  - *ACL*, 2023.

- Defending Against Backdoor Attacks in Natural Language Generation.  
  - Sun, Xiaofei, Li, Xiaoya, Meng, Yuxian, Ao, Xiang, Lyu, Lingjuan, Li, Jiwei, **and** Zhang, Tianwei  
  - *AAAI*, 2023.

- Parafuzz: An Interpretability-Driven Technique for Detecting Poisoned Samples in NLP.  
  - Yan, Lu, Zhang, Zhuo, Tao, Guanhong, Zhang, Kaiyuan, Chen, Xuan, Shen, Guangyu, **and** Zhang, Xiangyu  
  - *NeurIPS*, 2024.

- Defending Pre-Trained Language Models as Few-Shot Learners Against Backdoor Attacks.  
  - Xi, Zhaohan, Du, Tianyu, Li, Changjiang, Pang, Ren, Ji, Shouling, Chen, Jinghui, Ma, Fenglong, **and** Wang, Ting  
  - *NeurIPS*, 2024.

- Analyzing and Editing Inner Mechanisms of Backdoored Language Models.  
  - Lamparth, Max, **and** Reuel, Anka  
  - *ACM FAccT*, 2024.

- Backdoor Removal for Generative Large Language Models.  
  - Li, Haoran, Chen, Yulin, Zheng, Zihao, Hu, Qi, Chan, Chunkit, Liu, Heshan, **and** Song, Yangqiu  
  - *arXiv preprint arXiv:2405.07667*, 2024.

- Beear: Embedding-Based Adversarial Removal of Safety Backdoors in Instruction-Tuned Language Models.  
  - Zeng, Yi, Sun, Weiyu, Huynh, Tran Ngoc, Song, Dawn, Li, Bo, **and** Jia, Ruoxi  
  - *EMNLP*, 2024.

- CROW: Eliminating Backdoors from Large Language Models via Internal Consistency Regularization.  
  - Min, Nay Myat, Pham, Long H, Li, Yige, **and** Sun, Jun  
  - *arXiv preprint arXiv:2411.12768*, 2024.

- Setting the Trap: Capturing and Defeating Backdoors in Pretrained Language Models Through Honeypots.  
  - Tang, Ruixiang Ryan, Yuan, Jiayi, Li, Yiming, Liu, Zirui, Chen, Rui, **and** Hu, Xia  
  - *NeurIPS*, 2023.

- Maximum Entropy Loss, the Silver Bullet Targeting Backdoor Attacks in Pre-Trained Language Models.  
  - Liu, Zhengxiao, Shen, Bowen, Lin, Zheng, Wang, Fali, **and** Wang, Weiping  
  - *ACL*, 2023.

- Data-Centric NLP Backdoor Defense from the Lens of Memorization.  
  - Wang, Zhenting, Wang, Zhizhi, Jin, Mingyu, Du, Mengnan, Zhai, Juan, **and** Ma, Shiqing  
  - *arXiv preprint arXiv:2409.14200*, 2024.

- Securing Multi-Turn Conversational Language Models Against Distributed Backdoor Triggers.  
  - Tong, Terry, Xu, Jiashu, Liu, Qin, **and** Chen, Muhao  
  - *arXiv preprint arXiv:2407.04151*, 2024.

- CleanGen: Mitigating Backdoor Attacks for Generation Tasks in Large Language Models.  
  - Li, Yuetai, Xu, Zhangchen, Jiang, Fengqing, Niu, Luyao, Sahabandu, Dinuka, Ramasubramanian, Bhaskar, **and** Poovendran, Radha  
  - *EMNLP*, 2024.


##### Safety Alignment

- Deep Reinforcement Learning from Human Preferences.  
  - Christiano, Paul F., Leike, Jan, Brown, Tom, Martic, Miljan, Legg, Shane, **and** Amodei, Dario  
  - *NeurIPS*, 2017.

- Fine-Tuning Language Models from Human Preferences.  
  - Ziegler, Daniel M., Stiennon, Nisan, Wu, Jeffrey, Brown, Tom B., Radford, Alec, Amodei, Dario, Christiano, Paul, **and** Irving, Geoffrey  
  - *arXiv preprint arXiv:1909.08593*, 2019.

- Training Language Models to Follow Instructions with Human Feedback.  
  - Ouyang, Long, Wu, Jeffrey, Jiang, Xu, Almeida, Diogo, Wainwright, Carroll, Mishkin, Pamela, Zhang, Chong, Agarwal, Sandhini, Slama, Katarina, Ray, Alex, **et al.**  
  - *NeurIPS*, 2022.

- Safe RLHF: Safe Reinforcement Learning from Human Feedback.  
  - Dai, Josef, Pan, Xuehai, Sun, Ruiyang, Ji, Jiaming, Xu, Xinbo, Liu, Mickel, Wang, Yizhou, **and** Yang, Yaodong  
  - *ICLR*, 2024.

- Direct Preference-Based Policy Optimization Without Reward Modeling.  
  - An, Gaon, Lee, Junhyeok, Zuo, Xingdong, Kosaka, Norio, Kim, Kyung-Min, **and** Song, Hyun Oh  
  - *NeurIPS*, 2023.

- Direct Preference Optimization: Your Language Model is Secretly a Reward Model.  
  - Rafailov, Rafael, Sharma, Archit, Mitchell, Eric, Manning, Christopher D., Ermon, Stefano, **and** Finn, Chelsea  
  - *NeurIPS*, 2024.

- Beyond One-Preference-for-All: Multi-Objective Direct Preference Optimization.  
  - Zhou, Zhanhui, Liu, Jie, Yang, Chao, Shao, Jing, Liu, Yu, Yue, Xiangyu, Ouyang, Wanli, **and** Qiao, Yu  
  - *ACL*, 2024.

- KTO: Model Alignment as Prospect Theoretic Optimization.  
  - Ethayarajh, Kawin, Xu, Winnie, Muennighoff, Niklas, Jurafsky, Dan, **and** Kiela, Douwe  
  - *arXiv preprint arXiv:2402.01306*, 2024.

- LIMA: Less is More for Alignment.  
  - Zhou, Chunting, Liu, Pengfei, Xu, Puxin, Iyer, Srinivasan, Sun, Jiao, Mao, Yuning, Ma, Xuezhe, Efrat, Avia, Yu, Ping, Yu, Lili, **et al.**  
  - *NeurIPS*, 2024.

- Constitutional AI: Harmlessness from AI Feedback.  
  - Bai, Yuntao, Kadavath, Saurav, Kundu, Sandipan, Askell, Amanda, Kernion, Jackson, Jones, Andy, Chen, Anna, Goldie, Anna, Mirhoseini, Azalia, McKinnon, Cameron, **et al.**  
  - *arXiv preprint arXiv:2212.08073*, 2022.

- Principle-Driven Self-Alignment of Language Models from Scratch with Minimal Human Supervision.  
  - Sun, Zhiqing, Shen, Yikang, Zhou, Qinhong, Zhang, Hongxin, Chen, Zhenfang, Cox, David, Yang, Yiming, **and** Gan, Chuang  
  - *NeurIPS*, 2024.

- RLCD: Reinforcement Learning from Contrastive Distillation for LM Alignment.  
  - Yang, Kevin, Klein, Dan, Celikyilmaz, Asli, Peng, Nanyun, **and** Tian, Yuandong  
  - *ICLR*, 2024.

- Training Socially Aligned Language Models on Simulated Social Interactions.  
  - Liu, Ruibo, Yang, Ruixin, Jia, Chenyan, Zhang, Ge, Zhou, Denny, Dai, Andrew M., Yang, Diyi, **and** Vosoughi, Soroush  
  - *ICLR*, 2024.

- Self-Alignment of Large Language Models via Monopolylogue-Based Social Scene Simulation.  
  - Pang, Xianghe, Tang, Shuo, Ye, Rui, Xiong, Yuxin, Zhang, Bolun, Wang, Yanfeng, **and** Chen, Siheng  
  - *arXiv preprint arXiv:2402.05699*, 2024.


##### Energy Latency Attacks

- Nmtsloth: Understanding and Testing Efficiency Degradation of Neural Machine Translation Systems.  
  - Chen, Simin, Liu, Cong, Haque, Mirazul, Song, Zihe, **and** Yang, Wei  
  - *ESEC/FSE*, 2022.

- Dynamic Transformers Provide a False Sense of Efficiency.  
  - Chen, Yiming, Chen, Simin, Li, Zexin, Yang, Wei, Liu, Cong, Tan, Robby, **and** Li, Haizhou  
  - *ACL*, 2023.

- LLMEffiChecker: Understanding and Testing Efficiency Degradation of Large Language Models.  
  - Feng, Xiaoning, Han, Xiaohong, Chen, Simin, **and** Yang, Wei  
  - *ACM Transactions on Software Engineering and Methodology*, Vol. 33, p. 38, 2024.

- TTSlow: Slow Down Text-to-Speech with Efficiency Robustness Evaluations.  
  - Gao, Xiaoxue, Chen, Yiming, Yue, Xianghu, Tsao, Yu, **and** Chen, Nancy F.  
  - *arXiv preprint arXiv:2407.01927*, 2024.

- No-Skim: Towards Efficiency Robustness Evaluation on Skimming-Based Language Models.  
  - Zhang, Shengyao, Zhang, Mi, Pan, Xudong, **and** Yang, Min  
  - *arXiv preprint arXiv:2312.09494*, 2023.

- Denial-of-Service Poisoning Attacks Against Large Language Models.  
  - Gao, Kuofeng, Pang, Tianyu, Du, Chao, Yang, Yong, Xia, Shu-Tao, **and** Lin, Min  
  - *arXiv preprint arXiv:2410.10760*, 2024.


##### Model Extraction Attacks

- Lion: Adversarial Distillation of Proprietary Large Language Models.  
  - Jiang, Yuxin, Chan, Chunkit, Chen, Mingyang, **and** Wang, Wei  
  - *EMNLP*, 2023.

- On Extracting Specialized Code Abilities from Large Language Models: A Feasibility Study.  
  - Li, Zongjie, Wang, Chaozheng, Ma, Pingchuan, Liu, Chaowei, Wang, Shuai, Wu, Daoyuan, Gao, Cuiyun, **and** Liu, Yang  
  - *ICSE*, 2024.

- Alignment-Aware Model Extraction Attacks on Large Language Models.  
  - Liang, Zi, Ye, Qingqing, Wang, Yanyun, Zhang, Sen, Xiao, Yaxin, Li, Ronghua, Xu, Jianliang, **and** Hu, Haibo  
  - *arXiv preprint arXiv:2409.02718*, 2024.


##### Data Extraction Attacks

- The Secret Sharer: Evaluating and Testing Unintended Memorization in Neural Networks.  
  - Carlini, Nicholas, Liu, Chang, Erlingsson, Úlfar, Kos, Jernej, **and** Song, Dawn  
  - *USENIX Security*, 2019.

- Extracting Training Data from Large Language Models.  
  - Carlini, Nicholas, Tramer, Florian, Wallace, Eric, Jagielski, Matthew, Herbert-Voss, Ariel, Lee, Katherine, Roberts, Adam, Brown, Tom, Song, Dawn, Erlingsson, Ulfar, **et al.**  
  - *USENIX Security*, 2021.

- Scalable Extraction of Training Data from (Production) Language Models.  
  - Nasr, Milad, Carlini, Nicholas, Hayase, Jonathan, Jagielski, Matthew, Cooper, A Feder, Ippolito, Daphne, Choquette-Choo, Christopher A, Wallace, Eric, Tramèr, Florian, **and** Lee, Katherine  
  - *arXiv preprint arXiv:2311.17035*, 2023.

- Magpie: Alignment Data Synthesis from Scratch by Prompting Aligned LLMs with Nothing.  
  - Xu, Zhangchen, Jiang, Fengqing, Niu, Luyao, Deng, Yuntian, Poovendran, Radha, Choi, Yejin, **and** Lin, Bill Yuchen  
  - *arXiv preprint arXiv:2406.08464*, 2024.

- Traces of Memorisation in Large Language Models for Code.  
  - Al-Kaswan, Ali, Izadi, Maliheh, **and** Van Deursen, Arie  
  - *ICSE*, 2024.

- Special Characters Attack: Toward Scalable Training Data Extraction from Large Language Models.  
  - Bai, Yang, Pei, Ge, Gu, Jindong, Yang, Yong, **and** Ma, Xingjun  
  - *arXiv preprint arXiv:2405.05990*, 2024.

- Alpaca Against Vicuna: Using LLMs to Uncover Memorization of LLMs.  
  - Kassem, Aly M, Mahmoud, Omar, Mireshghallah, Niloofar, Kim, Hyunwoo, Tsvetkov, Yulia, Choi, Yejin, Saad, Sherif, **and** Rana, Santu  
  - *arXiv preprint arXiv:2403.04801*, 2024.

- Follow My Instruction and Spill the Beans: Scalable Data Extraction from Retrieval-Augmented Generation Systems.  
  - Qi, Zhenting, Zhang, Hanlin, Xing, Eric, Kakade, Sham, **and** Lakkaraju, Himabindu  
  - *arXiv preprint arXiv:2402.17840*, 2024.

- Towards More Realistic Extraction Attacks: An Adversarial Perspective.  
  - More, Yash, Ganesh, Prakhar, **and** Farnadi, Golnoosh  
  - *arXiv preprint arXiv:2407.02596*, 2024.

- Bag of Tricks for Training Data Extraction from Language Models.  
  - Yu, Weichen, Pang, Tianyu, Liu, Qian, Du, Chao, Kang, Bingyi, Huang, Yan, Lin, Min, **and** Yan, Shuicheng  
  - *ICML*, 2023.

- Uncovering Latent Memories: Assessing Data Leakage and Memorization Patterns in Large Language Models.  
  - Duan, Sunny, Khona, Mikail, Iyer, Abhiram, Schaeffer, Rylan, **and** Fiete, Ila R  
  - *ICML Workshop*, 2024.



</details>

<!-- Chapter 4-->
<details>

<summary><span id="ch4">Vision-Language Pre-training Model Safety</summary>

##### Adversarial Attacks

- Learning transferable visual models from natural language supervision.  
  - Radford, Alec, Kim, Jong Wook, Hallacy, Chris, Ramesh, Aditya, Goh, Gabriel, Agarwal, Sandhini, Sastry, Girish, Askell, Amanda, Mishkin, Pamela, Clark, Jack, **and others**  
  - *ICML*, 2021.

- Align before fuse: Vision and language representation learning with momentum distillation.  
  - Li, Junnan, Selvaraju, Ramprasaath, Gotmare, Akhilesh, Joty, Shafiq, Xiong, Caiming, **and** Hoi, Steven Chu Hong  
  - *NeurIPS*, 2021.

- Vision-language pre-training with triple contrastive learning.  
  - Yang, Jinyu, Duan, Jiali, Tran, Son, Xu, Yi, Chanda, Sampath, Chen, Liqun, Zeng, Belinda, Chilimbi, Trishul, **and** Huang, Junzhou  
  - *CVPR*, 2022.

- Fooling vision and language models despite localization and attention mechanism.  
  - Xu, Xiaojun, Chen, Xinyun, Liu, Chang, Rohrbach, Anna, Darrell, Trevor, **and** Song, Dawn  
  - *CVPR*, 2018.

- Cycle-consistency for robust visual question answering.  
  - Shah, Meet, Chen, Xinlei, Rohrbach, Marcus, **and** Parikh, Devi  
  - *CVPR*, 2019.

- BERT-ATTACK: Adversarial Attack Against BERT Using BERT.  
  - Li, Linyang, Ma, Ruotian, Guo, Qipeng, Xue, Xiangyang, **and** Qiu, Xipeng  
  - *EMNLP*, 2020.

- Defending multimodal fusion models against single-source adversaries.  
  - Yang, Karren, Lin, Wan-Yi, Barman, Manash, Condessa, Filipe, **and** Kolter, Zico  
  - *CVPR*, 2021.

- Towards adversarial attack on vision-language pre-training models.  
  - Zhang, Jiaming, Yi, Qi, **and** Sang, Jitao  
  - *ACM MM*, 2022.

- Advclip: Downstream-agnostic adversarial examples in multimodal contrastive learning.  
  - Zhou, Ziqi, Hu, Shengshan, Li, Minghui, Zhang, Hangtao, Zhang, Yechao, **and** Jin, Hai  
  - *ACM MM*, 2023.

- Reading Isn't Believing: Adversarial Attacks On Multi-Modal Neurons.  
  - Noever, David A, **and** Noever, Samantha E Miller  
  - *arXiv preprint arXiv:2103.10480*, 2021.

- Set-level guidance attack: Boosting adversarial transferability of vision-language pre-training models.  
  - Lu, Dong, Wang, Zhiqiang, Wang, Teng, Guan, Weili, Gao, Hongchang, **and** Zheng, Feng  
  - *ICCV*, 2023.

- Sa-attack: Improving adversarial transferability of vision-language pre-training models via self-augmentation.  
  - He, Bangyan, Jia, Xiaojun, Liang, Siyuan, Lou, Tianrui, Liu, Yang, **and** Cao, Xiaochun  
  - *arXiv preprint arXiv:2312.04913*, 2023.

- Exploring transferability of multimodal adversarial samples for vision-language pre-training models with contrastive learning.  
  - Wang, Youze, Hu, Wenbo, Dong, Yinpeng, Zhang, Hanwang, Su, Hang, **and** Hong, Richang  
  - *arXiv preprint arXiv:2308.12636*, 2023.

- Transferable multimodal attack on vision-language pre-training models.  
  - Wang, Haodi, Dong, Kai, Zhu, Zhilei, Qin, Haotong, Liu, Aishan, Fang, Xiaolin, Wang, Jiakai, **and** Liu, Xianglong  
  - *IEEE S&P*, 2024.

- VLATTACK: Multimodal Adversarial Attacks on Vision-Language Tasks via Pre-trained Models.  
  - Yin, Ziyi, Ye, Muchao, Zhang, Tianrong, Du, Tianyu, Zhu, Jinguo, Liu, Han, Chen, Jinghui, Wang, Ting, **and** Ma, Fenglong  
  - *NeurIPS*, 2023.

- As Firm As Their Foundations: Can open-sourced foundation models be used to create adversarial examples for downstream tasks?.  
  - Hu, Anjun, Gu, Jindong, Pinto, Francesco, Kamnitsas, Konstantinos, **and** Torr, Philip  
  - *arXiv preprint arXiv:2403.12693*, 2024.

- One Perturbation is Enough: On Generating Universal Adversarial Perturbations against Vision-Language Pre-training Models.  
  - Fang, Hao, Kong, Jiawei, Yu, Wenbo, Chen, Bin, Li, Jiawei, Xia, Shutao, **and** Xu, Ke  
  - *arXiv preprint arXiv:2406.05491*, 2024.

- Universal Adversarial Perturbations for Vision-Language Pre-trained Models.  
  - Zhang, Peng-Fei, Huang, Zi, **and** Bai, Guangdong  
  - *SIGIR*, 2024.


##### Adversarial Defenses

- MirrorCheck: Efficient Adversarial Defense for Vision-Language Models.  
  - Fares, Samar, Ziu, Klea, Aremu, Toluwani, Durasov, Nikita, Takáč, Martin, Fua, Pascal, Nandakumar, Karthik, **and** Laptev, Ivan  
  - *arXiv preprint arXiv:2406.09250*, 2024.

- AdvQDet: Detecting Query-Based Adversarial Attacks with Adversarial Contrastive Prompt Tuning.  
  - Wang, Xin, Chen, Kai, Ma, Xingjun, Chen, Zhineng, Chen, Jingjing, **and** Jiang, Yu-Gang  
  - *ACM MM*, 2024.

- Towards Deep Learning Models Resistant to Adversarial Attacks.  
  - Madry, Aleksander, Makelov, Aleksandar, Schmidt, Ludwig, Tsipras, Dimitris, **and** Vladu, Adrian  
  - *ICLR*, 2018.

- Reliable evaluation of adversarial robustness with an ensemble of diverse parameter-free attacks.  
  - Croce, Francesco, **and** Hein, Matthias  
  - *ICML*, 2020.

- Large-scale adversarial training for vision-and-language representation learning.  
  - Gan, Zhe, Chen, Yen-Chun, Li, Linjie, Zhu, Chen, Cheng, Yu, **and** Liu, Jingjing  
  - *NeurIPS*, 2020.

- FreeLB: Enhanced Adversarial Training for Natural Language Understanding.  
  - Zhu, Chen, Cheng, Yu, Gan, Zhe, Sun, Siqi, Goldstein, Tom, **and** Liu, Jingjing  
  - *ICLR*, 2020.

- Revisiting Adversarial Training at Scale.  
  - Wang, Zeyu, Li, Xianhang, Zhu, Hongru, **and** Xie, Cihang  
  - *CVPR*, 2024.

- Conditional prompt learning for vision-language models.  
  - Zhou, Kaiyang, Yang, Jingkang, Loy, Chen Change, **and** Liu, Ziwei  
  - *CVPR*, 2022.

- Learning to prompt for vision-language models.  
  - Zhou, Kaiyang, Yang, Jingkang, Loy, Chen Change, **and** Liu, Ziwei  
  - *International Journal of Computer Vision*, 130, 2337-2348, 2022.

- Maple: Multi-modal prompt learning.  
  - Khattak, Muhammad Uzair, Rasheed, Hanoona, Maaz, Muhammad, Khan, Salman, **and** Khan, Fahad Shahbaz  
  - *CVPR*, 2023.

- Adversarial prompt tuning for vision-language models.  
  - Zhang, Jiaming, Ma, Xingjun, Wang, Xin, Qiu, Lingyu, Wang, Jiaqi, Jiang, Yu-Gang, **and** Sang, Jitao  
  - *ECCV*, 2024.

- One prompt word is enough to boost adversarial robustness for pre-trained vision-language models.  
  - Li, Lin, Guan, Haoyan, Qiu, Jianing, **and** Spratling, Michael  
  - *CVPR*, 2024.

- MixPrompt: Enhancing Generalizability and Adversarial Robustness for Vision-Language Models via Prompt Fusion.  
  - Fan, Hao, Ma, Zhaoyang, Li, Yong, Tian, Rui, Chen, Yunli, **and** Gao, Chenlong  
  - *ICIC*, 2024.

- PromptSmooth: Certifying Robustness of Medical Vision-Language Models via Prompt Learning.  
  - Hussein, Noor, Shamshad, Fahad, Naseer, Muzammal, **and** Nandakumar, Karthik  
  - *MICCAI*, 2024.

- Defense-Prefix for Preventing Typographic Attacks on CLIP.  
  - Azuma, Hiroki, **and** Matsui, Yusuke  
  - *ICCV*, 2023.

- Few-Shot Adversarial Prompt Learning on Vision-Language Models.  
  - Zhou, Yiwei, Xia, Xiaobo, Lin, Zhiwei, Han, Bo, **and** Liu, Tongliang  
  - *NeurIPS*, 2024.

- Adversarial Prompt Distillation for Vision-Language Models.  
  - Luo, Lin, Wang, Xin, Zi, Bojia, Zhao, Shihao, **and** Ma, Xingjun  
  - *arXiv preprint arXiv:2411.15244*, 2024.

- TAPT: Test-Time Adversarial Prompt Tuning for Robust Inference in Vision-Language Models.  
  - Wang, Xin, Chen, Kai, Zhang, Jiaming, Chen, Jingjing, **and** Ma, Xingjun  
  - *arXiv preprint arXiv:2411.13136*, 2024.

- Understanding Zero-shot Adversarial Robustness for Large-Scale Models.  
  - Mao, Chengzhi, Geng, Scott, Yang, Junfeng, Wang, Xin, **and** Vondrick, Carl  
  - *ICLR*, 2023.

- Pre-trained model guided fine-tuning for zero-shot adversarial robustness.  
  - Wang, Sibo, Zhang, Jie, Yuan, Zheng, **and** Shan, Shiguang  
  - *CVPR*, 2024.

- Revisiting the Adversarial Robustness of Vision Language Models: a Multimodal Perspective.  
  - Zhou, Wanqi, Bai, Shuanghao, Zhao, Qibin, **and** Chen, Badong  
  - *arXiv preprint arXiv:2404.19287*, 2024.

- Robust CLIP: Unsupervised Adversarial Fine-Tuning of Vision Embeddings for Robust Large Vision-Language Models.  
  - Schlarmann, Christian, Singh, Naman Deep, Croce, Francesco, **and** Hein, Matthias  
  - *ICML*, 2024.


##### Backdoor & Poisoning Attacks

- Poisoning and Backdooring Contrastive Learning.  
  - Carlini, Nicholas, **and** Terzis, Andreas  
  - *ICLR*, 2022.

- Poisoning web-scale training datasets is practical.  
  - Carlini, Nicholas, Jagielski, Matthew, Choquette-Choo, Christopher A, Paleka, Daniel, Pearce, Will, Anderson, Hyrum, Terzis, Andreas, Thomas, Kurt, **and** Tramèr, Florian  
  - *IEEE S&P*, 2024.

- Badencoder: Backdoor attacks to pre-trained encoders in self-supervised learning.  
  - Jia, Jinyuan, Liu, Yupei, **and** Gong, Neil Zhenqiang  
  - *IEEE S&P*, 2022.

- Data Poisoning based Backdoor Attacks to Contrastive Learning.  
  - Zhang, Jinghuai, Liu, Hongbin, Jia, Jinyuan, **and** Gong, Neil Zhenqiang  
  - *CVPR*, 2024.

- Badclip: Dual-embedding guided backdoor attack on multimodal contrastive learning.  
  - Liang, Siyuan, Zhu, Mingli, Liu, Aishan, Wu, Baoyuan, Cao, Xiaochun, **and** Chang, Ee-Chien  
  - *CVPR*, 2024.

- BadCLIP: Trigger-Aware Prompt Learning for Backdoor Attacks on CLIP.  
  - Bai, Jiawang, Gao, Kuofeng, Min, Shaobo, Xia, Shu-Tao, Li, Zhifeng, **and** Liu, Wei  
  - *CVPR*, 2024.

- Data poisoning attacks against multimodal encoders.  
  - Yang, Ziqing, He, Xinlei, Li, Zheng, Backes, Michael, Humbert, Mathias, Berrang, Pascal, **and** Zhang, Yang  
  - *ICML*, 2023.



##### Backdoor & Poisoning Defenses


- CleanCLIP: Mitigating data poisoning attacks in multimodal contrastive learning.  
  - Bansal, Hritik, Singhi, Nishad, Yang, Yu, Yin, Fan, Grover, Aditya, **and** Chang, Kai-Wei  
  - *ICCV*, 2023.

- Better Safe than Sorry: Pre-training CLIP against Targeted Data Poisoning and Backdoor Attacks.  
  - Yang, Wenhan, Gao, Jingdong, **and** Mirzasoleiman, Baharan  
  - *ICML*, 2024.

- Robust contrastive language-image pretraining against data poisoning and backdoor attacks.  
  - Yang, Wenhan, Gao, Jingdong, **and** Mirzasoleiman, Baharan  
  - *NeurIPS*, 2024.

- Mudjacking: Patching Backdoor Vulnerabilities in Foundation Models.  
  - Liu, Hongbin, Reiter, Michael K., **and** Gong, Neil Zhenqiang  
  - *USENIX Security*, 2024.

- TIJO: Trigger inversion with joint optimization for defending multimodal backdoored models.  
  - Sur, Indranil, Sikka, Karan, Walmer, Matthew, Koneripalli, Kaushik, Roy, Anirban, Lin, Xiao, Divakaran, Ajay, **and** Jha, Susmit  
  - *ICCV*, 2023.

- SEER: Backdoor Detection for Vision-Language Models through Searching Target Text and Image Trigger Jointly.  
  - Zhu, Liuwan, Ning, Rui, Li, Jiang, Xin, Chunsheng, **and** Wu, Hongyi  
  - *AAAI*, 2024.

- Detecting Backdoor Samples in Contrastive Language Image Pretraining.  
  - Huang, Hanxun, Erfani, Sarah, Li, Yige, Ma, Xingjun, **and** Bailey, James  
  - *ICLR*, 2025.

- Detecting backdoors in pre-trained encoders.  
  - Feng, Shiwei, Tao, Guanhong, Cheng, Siyuan, Shen, Guangyu, Xu, Xiangzhe, Liu, Yingqi, Zhang, Kaiyuan, Ma, Shiqing, **and** Zhang, Xiangyu  
  - *CVPR*, 2023.



</details>


<!-- Chapter 5-->
<details>

<summary><span id="ch5">Vison Language Model Safety</summary>

##### Adversarial Attacks


- On the adversarial robustness of multi-modal foundation models.  
  - Schlarmann, Christian, **and** Hein, Matthias  
  - *ICCV*, 2023.

- Flamingo: a visual language model for few-shot learning.  
  - Alayrac, Jean-Baptiste, Donahue, Jeff, Luc, Pauline, Miech, Antoine, Barr, Iain, Hasson, Yana, Lenc, Karel, Mensch, Arthur, Millican, Katherine, Reynolds, Malcolm, **and others**  
  - *NeurIPS*, 2022.

- GPT-4 Technical Report.  
  - Achiam, Josh, Adler, Steven, Agarwal, Sandhini, Ahmad, Lama, Akkaya, Ilge, Aleman, Florencia Leoni, Almeida, Diogo, Altenschmidt, Janko, Altman, Sam, Anadkat, Shyamal, **and others**  
  - *arXiv preprint arXiv:2303.08774*, 2023.

- Adversarial Robustness for Visual Grounding of Multimodal Large Language Models.  
  - Gao, Kuofeng, Bai, Yang, Bai, Jiawang, Yang, Yong, **and** Xia, Shu-Tao  
  - *ICLR Workshop*, 2024.

- On the robustness of large multimodal models against image adversarial attacks.  
  - Cui, Xuanming, Aparcedo, Alejandro, Jang, Young Kyun, **and** Lim, Ser-Nam  
  - *CVPR*, 2024.

- An Image Is Worth 1000 Lies: Transferability of Adversarial Images across Prompts on Vision-Language Models.  
  - Luo, Haochen, Gu, Jindong, Liu, Fengyuan, **and** Torr, Philip  
  - *ICLR*, 2024.

- Stop Reasoning! When Multimodal LLM with Chain-of-Thought Reasoning Meets Adversarial Image.  
  - Wang, Zefeng, Han, Zhen, Chen, Shuo, Xue, Fan, Ding, Zifeng, Xiao, Xun, Tresp, Volker, **and** Gu, Jindong  
  - *COLM*, 2024.

- InstructTA: Instruction-Tuned Targeted Attack for Large Vision-Language Models.  
  - Wang, Xunguang, Ji, Zhenlan, Ma, Pingchuan, Li, Zongjie, **and** Wang, Shuai  
  - *arXiv preprint arXiv:2312.01886*, 2023.

- How Robust is Google's Bard to Adversarial Image Attacks?.  
  - Dong, Yinpeng, Chen, Huanran, Chen, Jiawei, Fang, Zhengwei, Yang, Xiao, Zhang, Yichi, Tian, Yu, Su, Hang, **and** Zhu, Jun  
  - *NeurIPS Workshop*, 2023.

- On evaluating adversarial robustness of large vision-language models.  
  - Zhao, Yunqing, Pang, Tianyu, Du, Chao, Yang, Xiao, Li, Chongxuan, Cheung, Ngai-Man Man, **and** Lin, Min  
  - *NeurIPS*, 2024.

- Learning transferable visual models from natural language supervision.  
  - Radford, Alec, Kim, Jong Wook, Hallacy, Chris, Ramesh, Aditya, Goh, Gabriel, Agarwal, Sandhini, Sastry, Girish, Askell, Amanda, Mishkin, Pamela, Clark, Jack, **and others**  
  - *ICML*, 2021.

- Blip-2: Bootstrapping language-image pre-training with frozen image encoders and large language models.  
  - Li, Junnan, Li, Dongxu, Savarese, Silvio, **and** Hoi, Steven  
  - *ICML*, 2023.

- Efficiently Adversarial Examples Generation for Visual-Language Models under Targeted Transfer Scenarios using Diffusion Models.  
  - Guo, Qi, Pang, Shanmin, Jia, Xiaojun, **and** Guo, Qing  
  - *arXiv preprint arXiv:2404.10335*, 2024.

- AnyAttack: Towards Large-scale Self-supervised Generation of Targeted Adversarial Examples for Vision-Language Models.  
  - Zhang, Jiaming, Ye, Junhong, Ma, Xingjun, Li, Yige, Yang, Yunfan, Sang, Jitao, **and** Yeung, Dit-Yan  
  - *arXiv preprint arXiv:2410.05346*, 2024.


##### Jailbreak Attacks


- Image hijacks: Adversarial images can control generative models at runtime.  
  - Bailey, Luke, Ong, Euan, Russell, Stuart, **and** Emmons, Scott  
  - *arXiv preprint arXiv:2309.00236*, 2023.

- Are aligned neural networks adversarially aligned?.  
  - Carlini, Nicholas, Nasr, Milad, Choquette-Choo, Christopher A, Jagielski, Matthew, Gao, Irena, Koh, Pang Wei W, Ippolito, Daphne, Tramer, Florian, **and** Schmidt, Ludwig  
  - *NeurIPS*, 2024.

- Visual adversarial examples jailbreak aligned large language models.  
  - Qi, Xiangyu, Huang, Kaixuan, Panda, Ashwinee, Henderson, Peter, Wang, Mengdi, **and** Mittal, Prateek  
  - *AAAI*, 2024.

- Jailbreaking attack against multimodal large language model.  
  - Niu, Zhenxing, Ren, Haodong, Gao, Xinbo, Hua, Gang, **and** Jin, Rong  
  - *arXiv preprint arXiv:2402.02309*, 2024.

- White-box Multimodal Jailbreaks Against Large Vision-Language Models.  
  - Wang, Ruofan, Ma, Xingjun, Zhou, Hanxu, Ji, Chuanjun, Ye, Guangnan, **and** Jiang, Yu-Gang  
  - *ACM MM*, 2024.

- Images are Achilles' Heel of Alignment: Exploiting Visual Vulnerabilities for Jailbreaking Multimodal Large Language Models.  
  - Li, Yifan, Guo, Hangyu, Zhou, Kun, Zhao, Wayne Xin, **and** Wen, Ji-Rong  
  - *ECCV*, 2024.

- Jailbreak in pieces: Compositional adversarial attacks on multi-modal language models.  
  - Shayegani, Erfan, Dong, Yue, **and** Abu-Ghazaleh, Nael  
  - *ICLR*, 2023.

- Figstep: Jailbreaking large vision-language models via typographic visual prompts.  
  - Gong, Yichen, Ran, Delong, Liu, Jinyuan, Wang, Conglei, Cong, Tianshuo, Wang, Anyu, Duan, Sisi, **and** Wang, Xiaoyun  
  - *AAAI*, 2025.

- Visual-RolePlay: Universal Jailbreak Attack on MultiModal Large Language Models via Role-playing Image Character.  
  - Ma, Siyuan, Luo, Weidi, Wang, Yu, Liu, Xiaogeng, Chen, Muhao, Li, Bo, **and** Xiao, Chaowei  
  - *arXiv preprint arXiv:2405.20773*, 2024.

- Jailbreaking GPT-4V via self-adversarial attacks with system prompts.  
  - Wu, Yuanwei, Li, Xiang, Liu, Yixin, Zhou, Pan, **and** Sun, Lichao  
  - *arXiv preprint arXiv:2311.09127*, 2023.

- IDEATOR: Jailbreaking VLMs Using VLMs.  
  - Wang, Ruofan, Wang, Bo, Ma, Xingjun, **and** Jiang, Yu-Gang  
  - *arXiv preprint arXiv:2411.00827*, 2024.


##### Jailbreak Defenses


- Adashield: Safeguarding multimodal large language models from structure-based attack via adaptive shield prompting.  
  - Wang, Yu, Liu, Xiaogeng, Li, Yu, Chen, Muhao, **and** Xiao, Chaowei  
  - *ECCV*, 2024.

- A mutation-based method for multi-modal jailbreaking attack detection.  
  - Zhang, Xiaoyu, Zhang, Cen, Li, Tianlin, Huang, Yihao, Jia, Xiaojun, Xie, Xiaofei, Liu, Yang, **and** Shen, Chao  
  - *arXiv preprint arXiv:2312.10766*, 2023.

- Defending Language Models Against Image-Based Prompt Attacks via User-Provided Specifications.  
  - Sharma, Reshabh K, Gupta, Vinayak, **and** Grossman, Dan  
  - *IEEE SPW*, 2024.

- MLLM-Protector: Ensuring MLLM's Safety without Hurting Performance.  
  - Pi, Renjie, Han, Tianyang, Xie, Yueqi, Pan, Rui, Lian, Qing, Dong, Hanze, Zhang, Jipeng, **and** Zhang, Tong  
  - *EMNLP*, 2024.

- Eyes closed, safety on: Protecting multimodal LLMs via image-to-text transformation.  
  - Gou, Yunhao, Chen, Kai, Liu, Zhili, Hong, Lanqing, Xu, Hang, Li, Zhenguo, Yeung, Dit-Yan, Kwok, James T, **and** Zhang, Yu  
  - *ECCV*, 2024.

- Inferaligner: Inference-time alignment for harmlessness through cross-model guidance.  
  - Wang, Pengyu, Zhang, Dong, Li, Linyang, Tan, Chenkun, Wang, Xinghao, Ren, Ke, Jiang, Botian, **and** Qiu, Xipeng  
  - *EMNLP*, 2024.

- BlueSuffix: Reinforced Blue Teaming for Vision-Language Models Against Jailbreak Attacks.  
  - Zhao, Yunhan, Zheng, Xiang, Luo, Lin, Li, Yige, Ma, Xingjun, **and** Jiang, Yu-Gang  
  - *ICLR*, 2025.


##### Energy Latency Attacks

- Inducing High Energy-Latency of Large Vision-Language Models with Verbose Images.  
  - Gao, Kuofeng, Bai, Yang, Gu, Jindong, Xia, Shu-Tao, Torr, Philip, Li, Zhifeng, **and** Liu, Wei  
  - *ICLR*, 2024.

##### Prompt Injection Attack

- (Ab) using Images and Sounds for Indirect Instruction Injection in Multi-Modal LLMs.  
  - Bagdasaryan, Eugene, Hsieh, Tsung-Yin, Nassi, Ben, **and** Shmatikov, Vitaly  
  - *arXiv preprint arXiv:2307.10490*, 2023.

- Vision-llms can fool themselves with self-generated typographic attacks.  
  - Qraitem, Maan, Tasnim, Nazia, Saenko, Kate, **and** Plummer, Bryan A  
  - *arXiv preprint arXiv:2402.00626*, 2024.

- Can language models be instructed to protect personal information?.  
  - Chen, Yang, Mendes, Ethan, Das, Sauvik, Xu, Wei, **and** Ritter, Alan  
  - *arXiv preprint arXiv:2310.02224*, 2023.


##### Backdoor & Poisoning Attacks

- Revisiting backdoor attacks against large vision-language models.  
  - Liang, Siyuan, Liang, Jiawei, Pang, Tianyu, Du, Chao, Liu, Aishan, Chang, Ee-Chien, **and** Cao, Xiaochun  
  - *arXiv preprint arXiv:2406.18844*, 2024.

- Physical Backdoor Attack can Jeopardize Driving with Vision-Large-Language Models.  
  - Ni, Zhenyang, Ye, Rui, Wei, Yuxi, Xiang, Zhen, Wang, Yanfeng, **and** Chen, Siheng  
  - *ICML Workshop*, 2024.

- ImgTrojan: Jailbreaking Vision-Language Models with ONE Image.  
  - Tao, Xijia, Zhong, Shuai, Li, Lei, Liu, Qi, **and** Kong, Lingpeng  
  - *arXiv preprint arXiv:2403.02910*, 2024.

- Test-time backdoor attacks on multimodal large language models.  
  - Lu, Dong, Pang, Tianyu, Du, Chao, Liu, Qian, Yang, Xianjun, **and** Lin, Min  
  - *arXiv preprint arXiv:2402.08577*, 2024.

- Shadowcast: Stealthy data poisoning attacks against vision-language models.  
  - Xu, Yuancheng, Yao, Jiarui, Shu, Manli, Sun, Yanchao, Wu, Zichu, Yu, Ning, Goldstein, Tom, **and** Huang, Furong  
  - *NeurIPS*, 2024.



</details>


<!-- Chapter 6-->
<details>

<summary><span id="ch6">Diffusion Models Safety</summary>

##### Adversarial Attacks

- Black Box Adversarial Prompting for Foundation Models.
  - Natalie Maus, Patrick Chao, Eric Wong, **and** Jacob R. Gardner
  - *NFAML*, 2023.

- A pilot study of query-free adversarial attack against stable diffusion.
  - Zhuang, Haomin, Zhang, Yihua, **and** Liu, Sijia
  - *CVPR*, 2023.

- Discovering Failure Modes of Text-guided Diffusion Models via Adversarial Search.
  - Qihao Liu, Adam Kortylewski, Yutong Bai, Song Bai, **and** Alan Yuille
  - *ICLR*, 2024.

- Discovering the hidden vocabulary of dalle-2.
  - Daras, Giannis **and** Dimakis, Alexandros G
  - *IJCAI*, 2022.

- Adversarial attacks on image generation with made-up words.
  - Milli{\`e
  - *arXiv preprint arXiv:2208.04135*, 2022.

- Revealing Vulnerabilities in Stable Diffusion via Targeted Attacks.
  - Zhang, Chenyu, Wang, Lanjun, **and** Liu, Anan
  - *arXiv preprint arXiv:2401.08725*, 2024.

- Stable diffusion is unstable.
  - Du, Chengbin, Li, Yanxi, Qiu, Zhongwei, **and** Xu, Chang
  - *NeurIPS*, 2024.


##### Jailbreak Attacks

- Sneakyprompt: Jailbreaking text-to-image generative models.
  - Yang, Yuchen, Hui, Bo, Yuan, Haolin, Gong, Neil, **and** Cao, Yinzhi
  - *IEEE S\&P*, 2024.

- Jailbreaking Text-to-Image Models with LLM-Based Agents.
  - Dong, Yingkai, Li, Zheng, Meng, Xiangtao, Yu, Ning, **and** Guo, Shanqing
  - *CCS*, 2024.

- SurrogatePrompt: Bypassing the Safety Filter of Text-To-Image Models via Substitution.
  - Ba, Zhongjie, Zhong, Jieming, Lei, Jiachen, Cheng, Peng, Wang, Qinglong, Qin, Zhan, Wang, Zhibo, **and** Ren, Kui
  - *CCS*, 2024.

- Prompting4debugging: Red-teaming text-to-image diffusion models by finding problematic prompts.
  - Chin, Zhi-Yi, Jiang, Chieh-Ming, Huang, Ching-Chun, Chen, Pin-Yu, **and** Chiu, Wei-Chen
  - *ICML*, 2024.

- Groot: Adversarial Testing for Generative Text-to-Image Models with Tree-based Semantic Transformation.
  - Liu, Yi, Yang, Guowei, Deng, Gelei, Chen, Feiyue, Chen, Yuqi, Shi, Ling, Zhang, Tianwei, **and** Liu, Yang
  - *arXiv preprint arXiv:2402.12100*, 2024.

- Divide-and-Conquer Attack: Harnessing the Power of LLM to Bypass the Censorship of Text-to-Image Generation Model.
  - Deng, Yimo **and** Chen, Huangxun
  - *arXiv preprint arXiv:2312.07130*, 2023.

- RT-Attack: Jailbreaking Text-to-Image Models via Random Token.
  - Gao, Sensen, Jia, Xiaojun, Huang, Yihao, Duan, Ranjie, Gu, Jindong, Liu, Yang, **and** Guo, Qing
  - *arXiv preprint arXiv:2408.13896*, 2024.

- Red-teaming the stable diffusion safety filter.
  - Rando, Javier, Paleka, Daniel, Lindner, David, Heim, Lennart, **and** Tram{\`e
  - *arXiv preprint arXiv:2210.04610*, 2022.


##### Jailbreak Defenses


- All but One: Surgical Concept Erasing with Model Preservation in Text-to-Image Diffusion Models.
  - Hong, Seunghoo, Lee, Juhun, **and** Woo, Simon S
  - *AAAI*, 2024.

- Receler: Reliable concept erasing of text-to-image diffusion models via lightweight erasers.
  - Huang, Chi-Pin, Chang, Kai-Po, Tsai, Chung-Ting, Lai, Yung-Hsuan, **and** Wang, Yu-Chiang Frank
  - *ECCV*, 2024.

- RACE: Robust Adversarial Concept Erasure for Secure Text-to-Image Diffusion Model.
  - Kim, Changhoon, Min, Kyle, **and** Yang, Yezhou
  - *ECCV*, 2024.

- Defensive Unlearning with Adversarial Training for Robust Concept Erasure in Diffusion Models.
  - Zhang, Yimeng, Chen, Xin, Jia, Jinghan, Zhang, Yihua, Fan, Chongyu, Liu, Jiancheng, Hong, Mingyi, Ding, Ke, **and** Liu, Sijia
  - *NeurIPS*, 2024.

- Degeneration-tuning: Using scrambled grid shield unwanted concepts from stable diffusion.
  - Ni, Zixuan, Wei, Longhui, Li, Jiacheng, Tang, Siliang, Zhuang, Yueting, **and** Tian, Qi
  - *ACM MM*, 2023.

- Implicit Concept Removal of Diffusion Models.
  - Liu, Zhili, Chen, Kai, Zhang, Yifan, Han, Jianhua, Hong, Lanqing, Xu, Hang, Li, Zhenguo, Yeung, Dit-Yan, **and** Kwok, J
  - *CVPR*, 2024.

- Mace: Mass concept erasure in diffusion models.
  - Lu, Shilin, Wang, Zilan, Li, Leyang, Liu, Yanzhu, **and** Kong, Adams Wai-Kin
  - *CVPR*, 2024.

- Unified concept editing in diffusion models.
  - Gandikota, Rohit, Orgad, Hadas, Belinkov, Yonatan, **and** Materzy{'n
  - *WACV*, 2024.

- Editing implicit assumptions in text-to-image diffusion models.
  - Orgad, Hadas, Kawar, Bahjat, **and** Belinkov, Yonatan
  - *ICCV*, 2023.

- Reliable and efficient concept erasure of text-to-image diffusion models.
  - Gong, Chao, Chen, Kai, Wei, Zhipeng, Chen, Jingjing, **and** Jiang, Yu-Gang
  - *ECCV*, 2024.

- ConceptPrune: Concept Editing in Diffusion Models via Skilled Neuron Pruning.
  - Chavhan, Ruchika, Li, Da, **and** Hospedales, Timothy
  - *NeurIPS*, 2024.

- Pruning for Robust Concept Erasing in Diffusion Models.
  - Tianyun Yang, Ziniu Li, Juan Cao, **and** Chang Xu
  - *Neurips Workshop*, 2024.

- Ethical-Lens: Curbing Malicious Usages of Open-Source Text-to-Image Models.
  - Cai, Yuzhu, Yin, Sheng, Wei, Yuxi, Xu, Chenxin, Mao, Weibo, Juefei-Xu, Felix, Chen, Siheng, **and** Wang, Yanfeng
  - *CVPR*, 2024.

- Self-discovering interpretable diffusion latent directions for responsible text-to-image generation.
  - Li, Hang, Shen, Chengzhi, Torr, Philip, Tresp, Volker, **and** Gu, Jindong
  - *CVPR*, 2024.

- Unlearning Concepts in Diffusion Model via Concept Domain Correction and Concept Preserving Gradient.
  - Wu, Yongliang, Zhou, Shiji, Yang, Mingzhuo, Wang, Lianzhe, Zhu, Wenbo, Chang, Heng, Zhou, Xiao, **and** Yang, Xu
  - *arXiv preprint arXiv:2405.15304*, 2024.

- Selective amnesia: A continual learning approach to forgetting in deep generative models.
  - Heng, Alvin **and** Soh, Harold
  - *NeurIPS*, 2024.

- Separable Multi-Concept Erasure from Diffusion Models.
  - Zhao, Mengnan, Zhang, Lihe, Zheng, Tianhang, Kong, Yuqiu, **and** Yin, Baocai
  - *arXiv preprint arXiv:2402.05947*, 2024.

- Continuous Concepts Removal in Text-to-image Diffusion Models.
  - Han, Tingxu, Sun, Weisong, Hu, Yanrong, Fang, Chunrong, Zhang, Yonglong, Ma, Shiqing, Zheng, Tao, Chen, Zhenyu, **and** Wang, Zhenting
  - *arXiv preprint arXiv:2412.00580*, 2024.

- RealEra: Semantic-level Concept Erasure via Neighbor-Concept Mining.
  - Liu, Yufan, An, Jinyang, Zhang, Wanqian, Li, Ming, Wu, Dayan, Gu, Jingzi, Lin, Zheng, **and** Wang, Weiping
  - *arXiv preprint arXiv:2410.09140*, 2024.

##### Backdoor Attacks

- How to backdoor diffusion models?.  
  - Chou, Sheng-Yen, Chen, Pin-Yu, **and** Ho, Tsung-Yi  
  - *CVPR*, 2023.

- Trojdiff: Trojan attacks on diffusion models with diverse targets.  
  - Chen, Weixin, Song, Dawn, **and** Li, Bo  
  - *CVPR*, 2023.

- Rickrolling the artist: Injecting backdoors into text encoders for text-to-image synthesis.  
  - Struppek, Lukas, Hintersdorf, Dominik, **and** Kersting, Kristian  
  - *ICCV*, 2023.

- Text-to-image diffusion models can be easily backdoored through multimodal data poisoning.  
  - Zhai, Shengfang, Dong, Yinpeng, Shen, Qingni, Pu, Shi, Fang, Yuejian, **and** Su, Hang  
  - *ACM MM*, 2023.

- Personalization as a shortcut for few-shot backdoor attack against text-to-image diffusion models.  
  - Huang, Yihao, Juefei-Xu, Felix, Guo, Qing, Zhang, Jie, Wu, Yutong, Hu, Ming, Li, Tianlin, Pu, Geguang, **and** Liu, Yang  
  - *AAAI*, 2024.

- From Trojan Horses to Castle Walls: Unveiling Bilateral Backdoor Effects in Diffusion Models.  
  - Pan, Zhuoshi, Yao, Yuguang, Liu, Gaowen, Shen, Bingquan, Zhao, H Vicky, Kompella, Ramana Rao, **and** Liu, Sijia  
  - *NeurIPS Workshop*, 2024.

- The stronger the diffusion model, the easier the backdoor: Data poisoning to induce copyright breaches without adjusting finetuning pipeline.  
  - Wang, Haonan, Shen, Qianli, Tong, Yao, Zhang, Yang, **and** Kawaguchi, Kenji  
  - *NeurIPS Workshop*, 2024.

- Villandiffusion: A unified backdoor attack framework for diffusion models.  
  - Chou, Sheng-Yen, Chen, Pin-Yu, **and** Ho, Tsung-Yi  
  - *NeurIPS*, 2024.

- Bagm: A backdoor attack for manipulating text-to-image generative models.  
  - Vice, Jordan, Akhtar, Naveed, Hartley, Richard, **and** Mian, Ajmal  
  - *IEEE Transactions on Information Forensics and Security*, 2024.

- Invisible Backdoor Attacks on Diffusion Models.  
  - Li, Sen, Ma, Junchi, **and** Cheng, Minhao  
  - *arXiv preprint arXiv:2406.00816*, 2024.

- Watch the Watcher! Backdoor Attacks on Security-Enhancing Diffusion Models.  
  - Li, Changjiang, Pang, Ren, Cao, Bochuan, Chen, Jinghui, Ma, Fenglong, Ji, Shouling, **and** Wang, Ting  
  - *arXiv preprint arXiv:2406.09669*, 2024.

- Injecting Bias in Text-To-Image Models via Composite-Trigger Backdoors.  
  - Naseh, Ali, Roh, Jaechul, Bagdasaryan, Eugene, **and** Houmansadr, Amir  
  - *arXiv preprint arXiv:2406.15213*, 2024.

- Zero-day backdoor attack against text-to-image diffusion models via personalization.  
  - Huang, Yihao, Guo, Qing, **and** Juefei-Xu, Felix  
  - *arXiv preprint arXiv:2305.10701*, 2023.


##### Backdoor Defenses

- T2IShield: Defending Against Backdoors on Text-to-Image Diffusion Models.  
  - Wang, Zhongqi, Zhang, Jie, Shan, Shiguang, **and** Chen, Xilin  
  - *ECCV*, 2024.

- Elijah: Eliminating backdoors injected in diffusion models via distribution shift.  
  - An, Shengwei, Chou, Sheng-Yen, Zhang, Kaiyuan, Xu, Qiuling, Tao, Guanhong, Shen, Guangyu, Cheng, Siyuan, Ma, Shiqing, Chen, Pin-Yu, Ho, Tsung-Yi, **and** others  
  - *AAAI*, 2024.

- TERD: A Unified Framework for Safeguarding Diffusion Models Against Backdoors.  
  - Mo, Yichuan, Huang, Hui, Li, Mingjie, Li, Ang, **and** Wang, Yisen  
  - *ICML*, 2024.

- UFID: A unified framework for input-level backdoor detection on diffusion models.  
  - Guan, Zihan, Hu, Mengxuan, Li, Sheng, **and** Vullikanti, Anil  
  - *arXiv preprint arXiv:2404.01101*, 2024.

- DisDet: Exploring Detectability of Backdoor Attack on Diffusion Models.  
  - Sui, Yang, Phan, Huy, Xiao, Jinqi, Zhang, Tianfang, Tang, Zijie, Shi, Cong, Wang, Yan, Chen, Yingying, **and** Yuan, Bo  
  - *arXiv preprint arXiv:2402.02739*, 2024.

- Diff-Cleanse: Identifying and Mitigating Backdoor Attacks in Diffusion Models.  
  - Hao, Jiang, Jin, Xiao, Xiaoguang, Hu, **and** Tianyou, Chen  
  - *arXiv preprint arXiv:2407.21316*, 2024.

- PureDiffusion: Using Backdoor to Counter Backdoor in Generative Diffusion Models.  
  - Truong, Vu Tuan, **and** Le, Long Bao  
  - *arXiv preprint arXiv:2409.13945*, 2024.

##### Membership Inference Attacks

- Generated distributions are all you need for membership inference attacks against generative models.  
  - Zhang, Minxing, Yu, Ning, Wen, Rui, Backes, Michael, **and** Zhang, Yang  
  - *CVPR*, 2024.

- Membership Inference on Text-to-Image Diffusion Models via Conditional Likelihood Discrepancy.  
  - Zhai, Shengfang, Chen, Huanran, Dong, Yinpeng, Li, Jiajun, Shen, Qingni, Gao, Yansong, Su, Hang, **and** Liu, Yang  
  - *NeurIPS*, 2024.

- Unveiling Structural Memorization: Structural Membership Inference Attack for Text-to-Image Diffusion Models.  
  - Li, Qiao, Fu, Xiaomeng, Wang, Xi, Liu, Jin, Gao, Xingyu, Dai, Jiao, **and** Han, Jizhong  
  - *ACM MM*, 2024.

- An Efficient Membership Inference Attack for the Diffusion Model by Proximal Initialization.  
  - Kong, Fei, Duan, Jinhao, Ma, RuiPeng, Shen, Heng Tao, Shi, Xiaoshuang, Zhu, Xiaofeng, **and** Xu, Kaidi  
  - *ICLR*, 2024.

- Towards more realistic membership inference attacks on large diffusion models.  
  - Dubiński, Jan, Kowalczuk, Antoni, Pawlak, Stanisław, Rokita, Przemyslaw, Trzciński, Tomasz, **and** Morawiecki, Paweł  
  - *WACV*, 2024.

- Membership inference attacks against diffusion models.  
  - Matsumoto, Tomoya, Miura, Takayuki, **and** Yanai, Naoto  
  - *SPW*, 2023.

- Are diffusion models vulnerable to membership inference attacks?.  
  - Duan, Jinhao, Kong, Fei, Wang, Shiqi, Shi, Xiaoshuang, **and** Xu, Kaidi  
  - *ICML*, 2023.

- Loss and Likelihood Based Membership Inference of Diffusion Models.  
  - Hu, Hailong, **and** Pang, Jun  
  - *ICIS*, 2023.

- Membership Inference Attacks Against Text-to-image Generation Models.  
  - Wu, Yixin, Yu, Ning, Li, Zheng, Backes, Michael, **and** Zhang, Yang  
  - *arXiv preprint arXiv:2210.00968*, 2022.

- Black-box membership inference attacks against fine-tuned diffusion models.  
  - Pang, Yan, **and** Wang, Tianhao  
  - *arXiv preprint arXiv:2312.08207*, 2023.

- Towards Black-Box Membership Inference Attack for Diffusion Models.  
  - Li, Jingwei, Dong, Jing, He, Tianxing, **and** Zhang, Jingzhao  
  - *arXiv preprint arXiv:2405.20771*, 2024.

- Model Will Tell: Training Membership Inference for Diffusion Models.  
  - Fu, Xiaomeng, Wang, Xi, Li, Qiao, Liu, Jin, Dai, Jiao, **and** Han, Jizhong  
  - *arXiv preprint arXiv:2403.08487*, 2024.

- Membership inference attacks on diffusion models via quantile regression.  
  - Tang, Shuai, Wu, Zhiwei Steven, Aydore, Sergul, Kearns, Michael, **and** Roth, Aaron  
  - *arXiv preprint arXiv:2312.05140*, 2023.

- A Probabilistic Fluctuation based Membership Inference Attack for Generative Models.  
  - Fu, Wenjie, Wang, Huandong, Gao, Chen, Liu, Guanghua, Li, Yong, **and** Jiang, Tao  
  - *arXiv preprint arXiv:2308.12143*, 2023.

- White-box membership inference attacks against diffusion models.  
  - Pang, Yan, Wang, Tianhao, Kang, Xuhui, Huai, Mengdi, **and** Zhang, Yang  
  - *arXiv preprint arXiv:2308.06405*, 2023.


##### Data Extraction Attacks

- Extracting training data from diffusion models.  
  - Carlini, Nicolas, Hayes, Jamie, Nasr, Milad, Jagielski, Matthew, Sehwag, Vikash, Tramer, Florian, Balle, Borja, Ippolito, Daphne, **and** Wallace, Eric  
  - *USENIX Security*, 2023.

- A reproducible extraction of training images from diffusion models.  
  - Webster, Ryan  
  - *arXiv preprint arXiv:2305.08694*, 2023.

- Towards a Theoretical Understanding of Memorization in Diffusion Models.  
  - Chen, Yunhao, Ma, Xingjun, Zou, Difan, **and** Jiang, Yu-Gang  
  - *arXiv preprint arXiv:2410.02467*, 2024.

- Revealing the Unseen: Guiding Personalized Diffusion Models to Expose Training Data.  
  - Wu, Xiaoyu, Zhang, Jiaru, **and** Wu, Steven  
  - *arXiv preprint arXiv:2410.03039*, 2024.

##### Model Extraction Attacks

- Recovering the Pre-Fine-Tuning Weights of Generative Models.  
  - Horwitz, Eliahu, Kahana, Jonathan, **and** Hoshen, Yedid  
  - *arXiv preprint arXiv:2402.10208*, 2024.

##### Intellectual Property Protection

- DUAW: Data-free Universal Adversarial Watermark against Stable Diffusion Customization.  
  - Ye, Xiaoyu, Huang, Hao, An, Jiaqi, **and** Wang, Yongtao  
  - *ICLR Workshop*, 2024.

- Adversarial example does good: Preventing painting imitation from diffusion models via adversarial examples.  
  - Liang, Chumeng, Wu, Xiaoyu, Hua, Yang, Zhang, Jiaru, Xue, Yiming, Song, Tao, Xue, Zhengui, Ma, Ruhui, **and** Guan, Haibing  
  - *ICML*, 2023.

- Anti-dreambooth: Protecting users from personalized text-to-image synthesis.  
  - Van Le, Thanh, Phung, Hao, Nguyen, Thuan Hoang, Dao, Quan, Tran, Ngoc N, **and** Tran, Anh  
  - *ICCV*, 2023.

- MetaCloak: Preventing Unauthorized Subject-driven Text-to-image Diffusion-based Synthesis via Meta-learning.  
  - Liu, Yixin, Fan, Chenrui, Dai, Yutong, Chen, Xun, Zhou, Pan, **and** Sun, Lichao  
  - *CVPR*, 2024.

- Countering Personalized Text-to-Image Generation with Influence Watermarks.  
  - Liu, Hanwen, Sun, Zhicheng, **and** Mu, Yadong  
  - *CVPR*, 2024.

- SimAC: A Simple Anti-Customization Method for Protecting Face Privacy against Text-to-Image Synthesis of Diffusion Models.  
  - Wang, Feifei, Tan, Zhentao, Wei, Tianyi, Wu, Yue, **and** Huang, Qidong  
  - *CVPR*, 2024.

- Editguard: Versatile image watermarking for tamper localization and copyright protection.  
  - Zhang, Xuanyu, Li, Runyi, Yu, Jiwen, Xu, Youmin, Li, Weiqi, **and** Zhang, Jian  
  - *CVPR*, 2024.

- A watermark-conditioned diffusion model for IP protection.  
  - Min, Rui, Li, Sen, Chen, Hongyang, **and** Cheng, Minhao  
  - *2024*, 2024.

- Watermark-embedded Adversarial Examples for Copyright Protection against Diffusion Models.  
  - Zhu, Peifei, Takahashi, Tsubasa, **and** Kataoka, Hirokatsu  
  - *CVPR*, 2024.

- Ft-shield: A watermark against unauthorized fine-tuning in text-to-image diffusion models.  
  - Cui, Yingqian, Ren, Jie, Lin, Yuping, Xu, Han, He, Pengfei, Xing, Yue, Fan, Wenqi, Liu, Hui, **and** Tang, Jiliang  
  - *arXiv preprint arXiv:2310.02401*, 2023.

- Diffusionshield: A watermark for copyright protection against generative diffusion models.  
  - Cui, Yingqian, Ren, Jie, Xu, Han, He, Pengfei, Liu, Hui, Sun, Lichao, Xing, Yue, **and** Tang, Jiliang  
  - *NeurIPS Workshop*, 2023.

- ProMark: Proactive Diffusion Watermarking for Causal Attribution.  
  - Asnani, Vishal, Collomosse, John, Bui, Tu, Liu, Xiaoming, **and** Agarwal, Shruti  
  - *CVPR*, 2024.

- Diagnosis: Detecting unauthorized data usages in text-to-image diffusion models.  
  - Wang, Zhenting, Chen, Chen, Lyu, Lingjuan, Metaxas, Dimitris N, **and** Ma, Shiqing  
  - *ICLR*, 2023.

- HiDDeN: Hiding Data With Deep Networks.  
  - Zhu, Jiren, Kaplan, Russell, Johnson, Justin, **and** Fei-Fei, Li  
  - *ECCV*, 2018.

- The stable signature: Rooting watermarks in latent diffusion models.  
  - Fernandez, Pierre, Couairon, Guillaume, Jégou, Hervé, Douze, Matthijs, **and** Furon, Teddy  
  - *ICCV*, 2023.

- LaWa: Using Latent Space for In-Generation Image Watermarking.  
  - Rezaei, Ahmad, Akbari, Mohammad, Alvar, Saeed Ranjbar, Fatemi, Arezou, **and** Zhang, Yong  
  - *ECCV*, 2024.

- Safe-SD: Safe and Traceable Stable Diffusion with Text Prompt Trigger for Invisible Generative Watermarking.  
  - Ma, Zhiyuan, Jia, Guoli, Qi, Biqing, **and** Zhou, Bowen  
  - *ACM MM*, 2024.

- A recipe for watermarking diffusion models.  
  - Zhao, Yunqing, Pang, Tianyu, Du, Chao, Yang, Xiao, Cheung, Ngai-Man, **and** Lin, Min  
  - *arXiv preprint arXiv:2303.10137*, 2023.

- Watermarking diffusion model.  
  - Liu, Yugeng, Li, Zheng, Backes, Michael, Shen, Yun, **and** Zhang, Yang  
  - *arXiv preprint arXiv:2305.12502*, 2023.

- Protecting the intellectual property of diffusion models by the watermark diffusion process.  
  - Peng, Sen, Chen, Yufei, Wang, Cong, **and** Jia, Xiaohua  
  - *arXiv preprint arXiv:2306.03436*, 2023.

- AquaLoRA: Toward White-box Protection for Customized Stable Diffusion Models via Watermark LoRA.  
  - Feng, Weitao, Zhou, Wenbo, He, Jiyan, Zhang, Jie, Wei, Tianyi, Li, Guanlin, Zhang, Tianwei, Zhang, Weiming, **and** Yu, Nenghai  
  - *ICML*, 2024.

- How to Trace Latent Generative Model Generated Images without Artificial Watermark?.  
  - Wang, Zhenting, Sehwag, Vikash, Chen, Chen, Lyu, Lingjuan, Metaxas, Dimitris N, **and** Ma, Shiqing  
  - *ICML*, 2024.

- Tree-ring watermarks: Fingerprints for diffusion images that are invisible and robust.  
  - Wen, Yuxin, Kirchenbauer, John, Geiping, Jonas, **and** Goldstein, Tom  
  - *NeurIPS*, 2023.




</details>


<!-- Chapter 7-->
<details>

<summary><span id="ch7">Agent Safety</summary>

##### LLM Agent

- Injecagent: Benchmarking indirect prompt injections in tool-integrated large language model agents.  
  - Zhan, Qiusi, Liang, Zhixiang, Ying, Zifan, **and** Kang, Daniel 
  - *ACL*, 2024.

- BadAgent: Inserting and Activating Backdoor Attacks in LLM Agents.  
  - Wang, Yifei, Xue, Dizhan, Zhang, Shengjie, **and** Qian, Shengsheng 
  - *ACL*, 2024.

- TrustAgent: Towards Safe and Trustworthy LLM-based Agents through Agent Constitution.  
  - Hua, Wenyue, Yang, Xianjun, Li, Zelong, Wei, Cheng, **and** Zhang, Yongfeng 
  - *ACL*, 2024.

- AutoDefense: Multi-Agent {LLM.  
  - Yifan Zeng, Yiran Wu, Xiao Zhang, Huazheng Wang, **and** Qingyun Wu 
  - *Neurips Workshop*, 2024.

- R-judge: Benchmarking safety risk awareness for llm agents.  
  - Yuan, Tongxin, He, Zhiwei, Dong, Lingzhong, Wang, Yiming, Zhao, Ruijie, Xia, Tian, Xu, Lizhen, Zhou, Binglin, Li, Fangqi, Zhang, Zhuosheng, **and** others 
  - *EMNLP*, 2024.

- AgentDojo: A Dynamic Environment to Evaluate Prompt Injection Attacks and Defenses for {LLM.  
  - Edoardo Debenedetti, Jie Zhang, Mislav Balunovic, Luca Beurer-Kellner, Marc Fischer, **and** Florian Tram{\`e 
  - *NeurIPS*, 2024.

- Breaking Agents: Compromising Autonomous LLM Agents Through Malfunction Amplification.  
  - Zhang, Boyang, Tan, Yicong, Shen, Yun, Salem, Ahmed, Backes, Michael, Zannettou, Savvas, **and** Zhang, Yang 
  - *arXiv preprint arXiv:2407.20859*, 2024.

- AgentPoison: Red-teaming LLM Agents via Poisoning Memory or Knowledge Bases.  
  - Chen, Zhaorun, Xiang, Zhen, Xiao, Chaowei, Song, Dawn, **and** Li, Bo 
  - *arXiv preprint arXiv:2407.12784*, 2024.

- Compromising Embodied Agents with Contextual Backdoor Attacks.  
  - Liu, Aishan, Zhou, Yuguang, Liu, Xianglong, Zhang, Tianyuan, Liang, Siyuan, Wang, Jiakai, Pu, Yanjun, Li, Tianlin, Zhang, Junqi, Zhou, Wenbo, **and** others 
  - *arXiv preprint arXiv:2408.02882*, 2024.

- Psysafe: A comprehensive framework for psychological-based attack, defense, and evaluation of multi-agent system safety.  
  - Zhang, Zaibin, Zhang, Yongting, Li, Lijun, Gao, Hongzhi, Wang, Lijun, Lu, Huchuan, Zhao, Feng, Qiao, Yu, **and** Shao, Jing 
  - *arXiv preprint arXiv:2401.11880*, 2024.

- GuardAgent: Safeguard LLM Agents by a Guard Agent via Knowledge-Enabled Reasoning.  
  - Xiang, Zhen, Zheng, Linzhi, Li, Yanjie, Hong, Junyuan, Li, Qinbin, Xie, Han, Zhang, Jiawei, Xiong, Zidi, Xie, Chulin, Yang, Carl, **and** others 
  - *arXiv preprint arXiv:2406.09187*, 2024.

- SafeAgentBench: A Benchmark for Safe Task Planning of Embodied LLM Agents.  
  - Yin, Sheng, Pang, Xianghe, Ding, Yuanzhuo, Chen, Menglan, Bi, Yutong, Xiong, Yichen, Huang, Wenhao, Xiang, Zhen, Shao, Jing, **and** Chen, Siheng 
  - *arXiv preprint arXiv:2412.13178*, 2024.


##### VLM Agent

- Agent smith: A single image can jailbreak one million multimodal llm agents exponentially fast.  
  - Gu, Xiangming, Zheng, Xiaosen, Pang, Tianyu, Du, Chao, Liu, Qian, Wang, Ye, Jiang, Jing, **and** Lin, Min 
  - *ICML*, 2024.

- Misusing tools in large language models with visual adversarial examples.  
  - Fu, Xiaohan, Wang, Zihan, Li, Shuheng, Gupta, Rajesh K, Mireshghallah, Niloofar, Berg-Kirkpatrick, Taylor, **and** Fernandes, Earlence 
  - *arXiv preprint arXiv:2310.03185*, 2023.

- The Wolf Within: Covert Injection of Malice into MLLM Societies via an MLLM Operative.  
  - Tan, Zhen, Zhao, Chengshuai, Moraffah, Raha, Li, Yifan, Kong, Yu, Chen, Tianlong, **and** Liu, Huan 
  - *arXiv preprint arXiv:2402.14859*, 2024.

- Adversarial Attacks on Multimodal Agents.  
  - Wu, Chen Henry, Koh, Jing Yu, Salakhutdinov, Ruslan, Fried, Daniel, **and** Raghunathan, Aditi 
  - *arXiv preprint arXiv:2406.12814*, 2024.
    

</details>


## 🥎 Open Challenges

Based on the survey, we identify several limitations and gaps in existing research and summarize them into the following topics. These open challenges reflect the evolving nature of large model safety, highlighting both technical and methodological barriers that must be overcome to ensure robustness and reliability across various AI systems.

<details>
  <summary>Fundamental Vulnerabilities</summary>

  **The Purpose of Attack Is Not Just to Break the Model**  
  While attacks are often designed to disrupt model functionality, they also serve as diagnostic tools to uncover unintended behaviors and reveal fundamental weaknesses. A deeper understanding of attack mechanisms can help address vulnerabilities at their root.

  **What Are the Fundamental Vulnerabilities of Language Models?**  
  LLMs are prone to adversarial inputs, biases, and prompt manipulation. Research must explore how these vulnerabilities stem from model architectures and training data to develop effective defenses.

  **How Vulnerabilities Propagate Across Modalities?**  
  As Multi-modal Large Language Models (MLLMs) integrate diverse modalities, new vulnerabilities arise. Vision encoders are known to be sensitive to subtle, continuous perturbations in pixel space, while language models are vulnerable to adversarial characters, words, or prompts. The interaction between modalities and how vulnerabilities in one modality propagate to others remains poorly understood.

  **Diffusion Models for Visual Content Generation Lack Language Capabilities**  
  Despite their success in visual content creation, diffusion models struggle with language comprehension, leading to unintended outputs. Integrating linguistic capabilities remains an open challenge.

  **How Much Training Data Can a Model Memorize?**  
  Deep neural networks exhibit memorization tendencies, raising privacy concerns. Understanding the mechanisms behind memorization is crucial for balancing performance and security.

  **Agent Vulnerabilities Grow with Their Abilities**  
  Large-model-powered agents face increasing vulnerabilities as their capabilities expand. Ensuring security in evolving agents requires comprehensive defense frameworks.

</details>

<details>
  <summary>Safety Evaluation</summary>

  **Attack Success Rate Is Not All We Need**  
  Metrics like attack success rate (ASR) fail to capture the full scope of safety risks. More comprehensive evaluation frameworks are needed to assess model resilience and ethical considerations.

  **Static Evaluations Create a False Sense of Safety**  
  Current safety benchmarks are static and may not reflect real-world threats. Dynamic evaluation methods are required to assess evolving risks effectively.

  **Adversarial Evaluations Are a Necessity, Not an Option**  
  Standard safety tests fail to capture adversarial risks. Adversarial evaluations are essential for understanding worst-case scenarios and improving robustness.

  **Open-Ended Evaluation**  
  LLMs generate open-ended responses, complicating attack assessments. Improved evaluation metrics and constrained output spaces are needed for accurate safety testing.

</details>

<details>
  <summary>Safety Defense</summary>

  **Safety Alignment Is Not the Savior**  
  Despite advances in safety alignment, models remain vulnerable to sophisticated attacks. Ensuring deeper, more robust alignment mechanisms is an ongoing challenge.

  **Jailbreak Attacks Are More Challenging to Defend Against Than Adversarial Attacks**  
  Jailbreak attacks bypass safety mechanisms more flexibly than traditional adversarial attacks. Defense strategies must account for unconstrained perturbations.

  **The Need for More Practical Defenses**  
  Effective defenses should be generalizable, efficient, black-box compatible, and adaptable to evolving threats.

  **The Lack of Proactive Defenses**  
  Current defenses focus on mitigating attacks post-occurrence. Proactive defense strategies could deter threats before they succeed.

  **Detection Has Been Overlooked in Current Defenses**  
  Detection mechanisms can enhance safety but are often neglected. Integrating detection into defense pipelines is a key research direction.

  **The Current Data Usage Practices Must Change**  
  Ethical and sustainable data usage is critical. Addressing concerns like consent, data attribution, and memorization is necessary for responsible AI deployment.

  **Safe Embodied Agents**  
  As AI extends into physical systems, ensuring safety in real-world interactions becomes paramount.

  **Safe Superintelligence**  
  Building safety mechanisms into AGI and superintelligent models is a critical challenge. Oversight systems, adversarial safety, and safety-conscious architectures are potential solutions.

</details>

<details>
  <summary>A Call for Collective Action</summary>

  **Defense-Oriented Research**  
  The focus on attack strategies has overshadowed the development of robust defenses. Research efforts should prioritize integrated, layered defense mechanisms.

  **Dedicated Safety APIs**  
  Commercial AI models should provide safety APIs to facilitate external safety evaluations and improvements.

  **Open-Source Platforms**  
  Developing and sharing safety platforms would foster collaboration, benchmarking, and transparency in AI safety research.

  **Global Collaborations**  
  AI safety is a global challenge requiring international cooperation in research, policy, and governance.

</details>


## 🐥 Citation

```bibtex
@article{ma2026safety,
  title={Safety at scale: A comprehensive survey of large model and agent safety},
  author={Ma, Xingjun and Gao, Yifeng and Wang, Yixu and Wang, Ruofan and Wang, Xin and Sun, Ye and Ding, Yifan and Xu, Hengyuan and Chen, Yunhao and Zhao, Yunhan and others},
  journal={Foundations and Trends in Privacy and Security},
  volume={8},
  number={3-4},
  pages={1--240},
  year={2026},
  publisher={Emerald Publishing Limited}
}

