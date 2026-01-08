# AI-Agent-Study
A whole workflow AI Agent Learning Journey

# Python setup
1. download Anaconda
2. download PyCharm
3. install libraries:
   1. pip install numpy pandas matplotlib seaborn scikit-learn tensorflow torch 
   2. pip install notebook jupyterlab
   3. PyTorch install: (python 3.11)
      1. For Nvidia GPU: conda install pytorch torchvision torchaudio pytorch-cuda=12.1 -c pytorch -c nvidia
      2. For CPU: conda install pytorch torchvision torchaudio -c pytorch 
4. Run it on local to install all packages:
   1. conda env create -f environment.yml
5. Check conda envs: conda info --envs
6. Switch env: conda activate torch(env name)
7. Terms:
   1. GPT: generative pre-trained transformers, model for text generation
   2. NLP: Natural language processing
   3. LLMs: Large Language models
      1. BERT: By directional encoder representation from transformers
      2. BART: By directional and autoregressive transformers 
      3. GPT:
      4. T5: Text to text transfer transformer
   4. RNNs: Recurrent neural networks, input,loop, output
   5. GANs: Generative adversarial networks, model for image/video generation
   6. VAEs: Variational autoencoders, art and creative design
   7. DALL-E: Data analysis learning with language model for generation and exploration, image
8. Models
   1. GANs: generator, Discriminator, competitive approach
   2. VAEs: characteristics-base
   3. A diffusion model, based on statistical properties. removing nosie and reconstructing distorted data, high-quality image
   4. RNNs: loop-based design, language model
   5. Transformers: self attention mechanism
   6. NLP: 
   7. RLHF: reinforcement learning from human feedback 
9. AI hallucinations
   1. AI hallucination can result in the generation of inaccurate information, the creation of biased views, and wrong input provided to sensitive applications.
   2. You can prevent the problems caused by AI hallucinations through:
      1. Extensive training with high-quality data,
      2. Avoiding manipulation,
      3. Ongoing evaluation and improvement of the models,
      4. Fine-tuning on domain-specific data,
      5. Being vigilant,
      6. Ensuring human oversight, and
      7. Providing additional context in the prompt.