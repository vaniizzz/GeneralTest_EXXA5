# GeneralTest_EXXA5
General Test

This test will focus on using computer vision techniques on synthetic observations produced from hydrodynamics simulations and radiative transfer calculations.

Overview

Protoplanetary disks are the sites of planet formation. The most recent generation of telescopes is able to resolve these objects in sufficient detail for the rigorous study of their properties, leading to a dramatic and rapid advancement in planet formation theory. Using synthetic observations that mimic data obtained from these observatories has allowed researchers to understand how specific conditions will manifest themselves in observations. See Terry et al. (2022) for an example of synthetic data creation and use.


Task

Using provided synthetic continuum observations of ALMA (1250 microns), found here, create a machine learning model capable of unsupervised clustering of the disks. No labels will be provided. The data is provided as .fits files, the standard format of observational data. Astropy is a particularly useful package for working with .fits data. Each image is a data cube containing 4 600x600 layers. Only the first one is relevant, i.e., index 0. 

The successful completion of this test will result in an automated pipeline of data loading, loading a trained model created by the participant, and passing the data through the model to create, label, and visualize clusters of the synthetic data. There are many ways in which this data can be clustered, but the number of planets/presence of any planets is of particular interest. Many of the images show clear signatures of one or more planets, so visual inspection is a useful tool. Beware of simply clustering the disks by viewing angle.

Deliverables

Script (ideally Jupyter Notebook) that includes the data-loading process and model creation, training, and testing. The script should be able to be run from start to finish without user intervention. It should produce clear plots that allow quick performance analysis. Data may be augmented in whatever manner you please, but that process should be automated to allow us to test using withheld data. Google Colab the preferred method of sharing the results.
If the training process is long, please deliver a pre-trained model of yours, ideally through a Google Drive. This is preferred regardless of training time in order to facilitate the evaluation of the task.

Metrics

Models will be judged on the clarity of clusters produced and the properties that the clusters find. The judges have all data pertaining to the disks and will run analyses of which properties are the most important in determining the clusters. Ideally, the clusters will correspond to properties pertaining to planets.

The quality of the cluster presentation and labeling will be taken into account. A clear presentation and data labeling that facilitates easy study will be judged highly.

The choice of model is of secondary importance to performance, but participants should use state-of-the-art models that are appropriate for this task.

Code should be clear, well-documented, and run without bugs or significant end-user modification.
