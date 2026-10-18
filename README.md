# EASY-IMAGE-GENERATOR
`EASY-IMAGE-GENERATOR` is a project that allows anyone to easily generate images using Google Colab.

## FEATURES
`EASY-IMAGE-GENERATOR` offers the following features.
- `EASY-IMAGE-GENERATOR` only requires a Google account to sign in. No other accounts are needed.
- `EASY-IMAGE-GENERATOR` is a free program that does not require an API key.
- `EASY-IMAGE-GENERATOR` allows you to train multiple models, including custom models based on your own artistic style.

## PROJECT STRUCTURE
`EASY-IMAGE-GENERATOR` is structured as follows.
```
EASY-IMAGE-GENERATOR/
├─ EASY-IMAGE-GENERATOR.ipynb
├─ LICENSE
└─ README.md
```

## EASY-IMAGE-GENERATOR.ipynb INFORMATION
`EASY-IMAGE-GENERATOR.ipynb` is a notebook used for model training and image generation.

`EASY-IMAGE-GENERATOR.ipynb` is structured as follows.
```
EASY-IMAGE-GENERATOR.ipynb
├─ TEXT CELL/
├─ CODE CELL 1/
│ ├─ INSTALL LIBRARY
│ ├─ IMPORT LIBRARY
│ ├─ DECLARE CONSTANT
│ ├─ DECLARE FUNCTION
│ ├─ MOUNT DRIVE
│ ├─ MAKE DIRECTORYS
│ └─ DOWNLOAD FILE
│
├─ CODE CELL 2/
│ └─ TRAIN MODEL
│
└─ CODE CELL 3/
  └─ GENERATE IMAGE
```

## USAGE
`EASY-IMAGE-GENERATOR` can be used as follows.
1. Prepare your text file and dataset.

	Your text file must follow the format below.
	```
	00.png: 20 years old, male, student
	01.png: 20 years old, female, student
	02.png: 30 years old, male, student
	```

2. Click the `Open in Colab` badge below.

	[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/YooJH0/EASY-IMAGE-GENERATOR/blob/main/EASY-IMAGE-GENERATOR.ipynb)

3. Run `CODE CELL 1`.

	Google Drive will be structured as follows.
	```
	EASY-IMAGE-GENERATOR/
	├─ dataset/
	├─ image/
	├─ model/
	├─ script/
	│ └─ train_text_to_image_lora.py
	│
	└─ text/
	```

4. Upload your text file to `text/` and your dataset to `dataset/`.

	Google Drive will be structured as follows.
	```
	EASY-IMAGE-GENERATOR/
	├─ dataset/
	│ └─ my_dataset/
	│   ├─ 00.png
	│   ├─ 01.png
	│   └─ 02.png
	│
	├─ image/
	├─ model/
	├─ script/
	│ └─ train_text_to_image_lora.py
	│
	└─ text/
	  └─ my_text.txt
	```

5. Modify `CODE CELL 2` and `CODE CELL 3` to suit your needs.

6. Run `CODE CELL 2` and `CODE CELL 3`.

	Google Drive will be structured as follows.
	```
	EASY-IMAGE-GENERATOR/
	├─ dataset/
	│ └─ my_dataset/
	│   ├─ 00.png
	│   ├─ 01.png
	│   ├─ 02.png
	│   └─ metadata.jsonl
	│
	├─ image/
	│ └─ my_image.png
	│
	├─ model/
	│ └─ my_model/
	│   ├─ logs/
	│   └─ pytorch_lora_weights.safetensors
	│
	├─ script/
	│ └─ train_text_to_image_lora.py
	│
	└─ text/
	  └─ my_text.txt
	```

## CONTRIBUTING
1. Create a new branch.
	```
	git checkout -b <branch-name>
	```

2. Stage your changes.
	```
	git add .
	```

3. Commit your changes.
	```
	git commit -m "<commit-message>"
	```

4. Push your branch.
	```
	git push -u origin <branch-name>
	```

5. Open a pull request.

## LICENSE
`EASY-IMAGE-GENERATOR` is licensed under the MIT License.

## AUTHORS
- Yoo, J. H.
	- [GitHub](https://github.com/YooJH0/)