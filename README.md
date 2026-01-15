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
      3. GPT:  Text generation
      4. T5: Text to text transfer transformer
   4. RNNs: Recurrent neural networks, input,loop, output
   5. GANs: Generative adversarial networks, model for image/video generation
   6. VAEs: Variational autoencoders, art and creative design
   7. DALL-E: Data analysis learning with language model for generation and exploration, image
8. Models
   1. GANs: generator, Discriminator, competitive approach
   2. VAEs: variational autoencoders, characteristics-base; operate on an encoder-decoder framework and create samples based on similar characteristics
   3. A diffusion model, based on statistical properties. removing nosie and reconstructing distorted data, high-quality image
   4. RNNs: use sequential or time series data and a loop-based design, language model
   5. Transformers: self attention mechanism
   6. NLP: 
   7. RLHF: reinforcement learning from human feedback
   8. WaveNet: natural-sounding speech
   9. Generative AI: deep-learning models, which can generate content based on the training data.
      1. understand the relationship between words and phrases and generate contextually relevant text
      2. started with rule-based systems that use predefined linguistic rules, followed by machine-learning approaches focusing on statistical methods. 
      3. It later moved to deep learning, which uses neural networks trained on extensive data sets.
      4. Transformers represent the latest in this evolution.
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
10. Libraries and tools
    1. PyTorch: Meta, dynamic computation graphs, deep learning
    2. TensorFlow: Google, machine learning and deep learning
       1. sentiment analysis, text classification, machine translation
       2. TFX: ML deployment pipeline(defining, launching, monitoring)
       3. Keras: high-level neural networks API
    3. Hugging face: Open-source with pretrained models and tools, streamline, fine-tuning
       1. The Model Hub: online platform with pretrained machine learning models
       2. Transformers(library): pretrained models for text
       3. Datasets(library): 
       4. Tokenizers(library): needed models like BERT and GPT
    4. LangChain: Open-source
       1. Advanced prompt engineering, specific inputs used to guid the model's behavior.
       2. Seamless integration with leading models
          1. GPT
       3. Application in NLP, ideal for creating tools: interactive chatbots & intricate analytical tools.
    5. Pydantic: streamline data handling, uses Python-type annotations
       1. Data validation: use BaseModel class to define data models and validations
       2. Settings: application settings and env variables
       3. Validating and managing data in NLP pipelines, ensures data integrity and consistency
11. Tokenization: Process of breaking a sentence into smaller pieces, or tokens.
    1. prepare data for training LLMs
       1. Implement tokenization
       2. Build data loaders
       3. Tokenization methods
          1. word based: preserve the semantic meaning but increases the model's vocabulary, problem: words with similar meanings will be assigned different IDs, treated as entirely separate words with distinct meanings.
          2. character based: increases input dimensionality and computational needs
          3. subword based: frequently used words can remain unsplit while infrequent words are broken down into meaningful sub words
             1. the word piece: splitting and merging two symbols to ensure its decisions are valuable
             2. unigram: breaks text into smaller pieces. gradually narrowing down possibilities. 
             3. sentence piece algorithms: text into manageable parts and assigns unique IDs.
       4. How tokenizers convert raw text into model input.
          1. 
       5. implement by using NLTK, spaCy, BertTokenizer, XLNetTokenizer
       6. Role of data loaders in the training pipeline
          1. how they batch, shuffle, and feed data to models
       7. PyTorch.DataLoader
       8. Key factors that contribute to data quality and diversity
       9. Tokenizer: breaks down text into individual tokens.
          1. NLTK and spaCy generate tokens
          2. NLTK: text processing and analysis
          3. spaCy: open-source library for advanced natural language processing. Speed and accuracy in processing large volumes of text data.
          4. BertTokenizer: Hugging Face Transformers library for working with state-of-the-art pre-trained language models. for BERT models
          5. XLNetTokenizer: Hugging Face Transformers library. For tokenizing text in alignment with the XLNet model's requirements.
          6. torchtext:PyTorch ecosystem, various natural language processing tasks.Simplifies the process of working with text datda and provides functions for data preprocessing, tokenization, vocabulary management, and btaching.