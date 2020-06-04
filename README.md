

# Endsem Project : Detection of Depression using Natural language Processing 

### Stephen Fernandes : UR16CS057

## Introduction :
 This Project is based upon detecting depression in textual data using Natual Lanuguage Processing techniques, an NLP Model BERT is used called Bi-directional Encoded Representational Trasnformer . it makes the used of attention mechanisim and word embeddings to train an NLp classifier into processing distinct NLP data . 
we used the BERT uncased pre built mode and further fine tune it to build our Depression Detection system . 

## instructions :
1. Make new Conda environment using Ananconda Package manager ( assuming you have Anaconda installed )
```bash
conda create --name mycondaenv python=3.6
```

 2. Activate the conda Environment 
```bash
conda activate mycondaenv
```

3. Install the Required Dependencies :
```bash
pip install pytorch==latest
```
```bash
pip install torchvision
```

```bash
pip install flask
```

```bash
pip install transformers==latest
```

 4. Navigate to the `src/` directory where the source python files are located : 
```bash
cd src/
```

5. Here the `train.py` file is used to train the model and the `app.py` file is used to deploy the model as a API 
to train the model , ensure your GPU is enabled by 
```bash 
nvidia-smi
```

and train the model by 

```bash
python train.py
```

6. To launch the model into the api production launch the fask app by :
 ```bash
python app.py
,,,

7. Note: Other files like `config.py` , `dataset.py`, `engine.py` are utility files that can be used to change and alter the Model configurations and arcitecture 

