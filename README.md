# neural_networks

# hw1
anaconda 安装keras：
Environments -> base(root）->  terminal -> pip install keras 
-> back to the environment base not installed -> choose keras -> apply


# hw2
when using the 
plt.plot(epochs, acc, 'bo', label='Training acc')
plt.plot(epochs, val_acc, 'b', label='Validation acc')
has following error:
OMP: Error #15: Initializing libiomp5.dylib, but found libiomp5.dylib already initialized.
there are two ways to solve it:
conda install nomkl
OR
import os
os.environ['KMP_DUPLICATE_LIB_OK']='True'

In addition, the epochs and acc must be array or scalar, range(1,2) might does not work
