# Awesome-Large-Model-Safety
## Safety at Scale: A Comprehensive Survey of Large Model Safety

--- 

Content:

- [Vision Foundation Model Safety](#ch2)
- [Large Language Model Safety](#ch3)
- [Vision-Language Pre-training Model Safety](#ch4)
- [Vison Language Model Safety](#ch5)
- [Diffusion Models Safety](#ch6)
- [Agent Safety](#ch7)

---
<!-- Chapter 2-->
<details>

<summary><span id="ch2">Vision Foundation Model Safety </span></summary>

##### Attacks and Defense for ViT
- Patch-fool: Are vision transformers always robust against adversarial perturbations?
    - Yonggan Fu, Shunyao Zhang, Shang Wu, Cheng Wan, Yingyan Celine Lin
    - [ICLR 2022](https://arxiv.org/pdf/2203.08392)

##### Attacks and Defense for SAM


</details>


<!-- Chapter 3-->
<details>

<summary><span id="ch3">Large Language Model Safety</summary>

##### Adversarial Attack

- Bad Characters: Imperceptible NLP Attacks
    - Nicholas Boucher, Ilia Shumailov, Ross Anderson, Nicolas Papernot
    - [S&P 2022](https://arxiv.org/abs/2106.09898)

##### Adversarial Defense

##### Jailbreak Attack

##### Jailbreak Defense

##### Prompt Injection Attacks

##### Prompt Injection Defenses

##### Backdoor Attacks

##### Backdoor Defenses

##### Safety Alignment

##### Energy Latency Attacks

##### Model Extraction Attacks

##### Data Extraction Attacks

</details>

<!-- Chapter 4-->
<details>

<summary><span id="ch4">Vision-Language Pre-training Model Safety</summary>

##### Adversarial Attacks
- Towards Adversarial Attack on Vision-Language Pre-training Models
    - Jiaming Zhang, Qi Yi, Jitao Sang
    - [S&P 2022](https://arxiv.org/abs/2106.09898)

##### Adversarial Defenses

##### Backdoor & Poisoning Attacks

##### Backdoor & Poisoning Defenses


</details>


<!-- Chapter 5-->
<details>

<summary><span id="ch5">Vison Language Model Safety</summary>

##### Adversarial Attacks

##### Jailbreak Attacks

##### Jailbreak Defenses

##### Energy Latency Attacks

##### Prompt Injection Attack

##### Backdoor & Poisoning Attacks

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
