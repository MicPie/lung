# lung
Lung fibrosis and inflammation CNN

The notebooks use the [dataset](https://osf.io/28qbc/) from the publication "[Deep neural network based histological scoring of lung fibrosis and inflammation in the mouse model system](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0202708)" to train CNNs based on different ResNet architectures to characterize fibrotic and inflammatory lung diseases from sections of lung tissue.

Notebooks:
* [lung_inflammation_v3_progressive-resizing-ResNet34.ipynb](https://github.com/MicPie/lung/blob/master/lung_inflammation_v3_progressive-resizing-ResNet34.ipynb) ([nbviewer](https://nbviewer.jupyter.org/github/MicPie/lung/blob/master/lung_inflammation_v3_progressive-resizing-ResNet34.ipynb)): Uses the trained weights from the [ResNet34 from below](https://github.com/MicPie/lung/blob/master/lung_inflammation_v2_from-folder-ResNet34.ipynb) and increases the image size to 512 ("progressive resizing"). This approach could improve the inflammatory accuracy benchmark from the publication by approx. 2%.
* [lung_inflammation_v2_from-folder-ResNet34.ipynb](https://github.com/MicPie/lung/blob/master/lung_inflammation_v2_from-folder-ResNet34.ipynb) ([nbviewer](https://nbviewer.jupyter.org/github/MicPie/lung/blob/master/lung_inflammation_v2_from-folder-ResNet34.ipynb)): Uses a ResNet34 architecture and slightly improves the inflammatory accuracy benchmark from the publication.
* [lung_inflammation_v2_from-folder-ResNet18.ipynb](https://github.com/MicPie/lung/blob/master/lung_inflammation_v2_from-folder-ResNet18.ipynb) ([nbviewer](https://nbviewer.jupyter.org/github/MicPie/lung/blob/master/lung_inflammation_v2_from-folder-ResNet18.ipynb)): Uses a ResNet18 architecture and achieves a similar inflammatory accuracy benchmark compared to the publication.


Deprecated notebooks:
* [lung_inflammation_v1_from-df.ipynb]() ([nbviewer](https://nbviewer.jupyter.org/github/MicPie/lung/blob/master/lung_inflammation_v1_from-df.ipynb)): Uses deprecated version of the fastai library.
