

## Human evaluation for three models generated results in MultiWoZ 2.1 dataset

### Data format

```json
[
{
	'dialogue history':'',   ## the input the model 
	'model1':{
	'output':'', 			 ## the generated result of model1
	'satisfaction score':'', ## TOB evaluated
	'semantic quality':''    ## TOB evaluated
	},
	'model2':{
	'output':'', 			 ## the generated result of model1
	'satisfaction score':'',
	'semantic quality':''
	},
	'model3':{
	'output':'', 			 ## the generated result of model1
	'satisfaction score':'', ## TOB evaluated
	'semantic quality':''    ## TOB evaluated
	}
}
]
```


### The criteria for satisfaction score and setimant quality

The satisfaction score range from 1-5, and you should mark a integer

- 1: Very dissatisfied (the system fails to understand and fulfill user’s request); 

- 2: Dissatisfied (the system understands the request but fails to satisfy it in any way); 

- 3: Normal (the system understands users request and either partially satisfies the request or provides information on how the request can be fulfilled); 

- 4: Satisfied (the system understands and satisfies the user request, but provides more information than what the user requested or takes
extra turns before meeting the request);

- 5: Very satisfied (the system understands and satisfies the user request completely and efficiently)

The semantic quality is determined by the fluency and coherence, ranging from 1 to 10. A score of 5 represents normal fluency and coherence.

### How to mark your score.

All you need to do is fill in the blank values for 'satisfaction score' and 'semantic quality'. Subsequently, the researchers will calculate the overall performance of different models.
