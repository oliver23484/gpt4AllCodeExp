# Information about the machine used to train the LLM with our own code files on top of its pre trained model : - 
## Trial 1 : - 
### GPU Based Local System Training
GPU - 6GB Vram (Nvidia RTX 3060 mobile) <br />
CUDA Version - 12 <br />
Cuda Cores - 3840 <br />
RAM - 16GB Memory <br />

Conclusion - The training failed throwing a memory error. The recommended VRAM in documentation is 8GB. <br />


## Trial 2 : - 
### GPU Based goole colab training
GPU - Tesla T4 <br />
RAM - 12 GB Memory <br />

Conclusion - The training crashed and runtime/kernel got disconnected. Tried multiple times. Also, uploading a 8 GB pre trained model to the colab workspace was taking forever so had to mount the google drive to refer to the model file. <br />


## Trial 3 : - 
### CPU Based Local System Training
CPU - 17-12700H (H-High Performance Graphics Version of the CPU.) <br />
Base Speed of CPU - 2.3 GHz <br />
Cores - 16 <br />
RAM - 16 GB Memory <br />

Conclusion - The training was successful and were able to get inferences. The general inference time is about 2 minutes. It can be improved by using GPU based training and inferenece. Also,it creates indexed of each query so that
next time when that query is entered it returns the results in seconds. Also, the returned response has fils names for reference of the response.
