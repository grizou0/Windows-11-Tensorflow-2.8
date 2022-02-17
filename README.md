# Windows-11-Tensorflow-2.8
PreInstallation
Visual Studio
Cuda 11.0 et CudNN V8 (on copie les fichers CudNN dans le repertoire Cuda)
anaconda3

# dépendances:
pip install tensorflow-gpu
pip install pandas
pip install matplotlib
pip install opencv-python
pip install tensorflow-hub
pip install tf_slim
pip install pycocotools
pip install lvis
pip install tensorflow_io
pip install tf-model-official
pip install glob2
(pour desinstaller, faire: pip uinstall moddul)

On vérifie les versions
python --version   
->3.9

#Installer le model et compilation
git clone https://github.com/tensorflow/models.git
La commabde git doit être préalablement installée
Dans le répertoire Tensorflow, on crée un répertoire scritps et workspace
Tensorflow
  -models
    -research
  -script
  -workspace
 Se placer dans le répertoire research et installer protobuf
 conda install -c anaconda protobuf
 Ensuite in compile:
 protoc object_detection\protos\*.proto --python_out=.
 
 pip install cython
 pip install git+https://github.com/philferriere/cocoapi.git#subdirectory=PythonAPI
 
 #On install et compile le paquet tensorflow 2
 Test du model
-------------
python object_detection\builders\model_builder_tf2_test.py

->
Ran 24 tests in 17.904s

OK (skipped=1)
#----------------------------------------------------------------------------


