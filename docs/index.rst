.. ChemML documentation master file, created by
   sphinx-quickstart on Thu Jun  2 13:42:11 2016.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

|logo|

Welcome to the ChemML's documentation!
======================================
ChemML is a machine learning and informatics program suite for the analysis, mining, and modeling of chemical and materials data.

    - source repository on github: https://github.com/hachmannlab/chemml

Code Design:
++++++++++++
ChemML is developed in the Python 3 programming language and makes use of a host of data analysis and ML libraries(accessible through the Anaconda distribution), as well as domain-specific libraries.
The development follows a strictly modular and object-oriented design to make the overall code as flexible and versatile as possible.

The format of library is similar to the well known libraries like Scikit-learn. ChemML will be soon available
via graphical user interface provided by [ChemEco](https://github.com/hachmannlab/chemeco).
ChemEco is a general-purpose framework for data mining without coding. It also interfaces with many of the libraries that supply methods for the
representation, preprocessing, analysis, mining, and modeling of large-scale chemical data sets.

Latest Version:
+++++++++++++++
   - to find the latest version and release history, click here: https://pypi.org/project/chemml/#history

Installation and Dependencies:
++++++++++++++++++++++++++++++
You can download ChemML from Python Package Index (PyPI) via pip.

.. code:: bash

    pip install chemml --user -U

Here is a list of external libraries that will be installed with chemml:
   - numpy
   - pandas
   - tensorflow
   - scikit-learn
   - matplotlib
   - seaborn
   - lxml

Since conda installation is not available for ChemML yet, we recommend installing rdkit and openbabel (please install Openbabel 2.x not Openbabel 3.xin a conda virtual environment prior to
installing ChemML. For doing so, you need to follow the conda installer:

.. code:: bash

    conda create --name my_chemml_env python=3.6
    source activate my_chemml_env
    conda install -c openbabel openbabel
    conda install -c conda-forge rdkit
    pip install chemml


Citation:
+++++++++
Please cite the use of ChemML as:

::

    Main citation:

    @article{chemml2019,
    author = {Haghighatlari, Mojtaba and Vishwakarma, Gaurav and Altarawy, Doaa and Subramanian, Ramachandran and Kota, Bhargava Urala and Sonpal, Aditya and Setlur, Srirangaraj and Hachmann, Johannes},
    journal = {ChemRxiv},
    pages = {8323271},
    title = {ChemML: A Machine Learning and Informatics Program Package for the Analysis, Mining, and Modeling of Chemical and Materials Data},
    doi = {10.26434/chemrxiv.8323271.v1},
    year = {2019}
    }


    Other references:

    @article{chemml_review2019,
    author = {Haghighatlari, Mojtaba and Hachmann, Johannes},
    doi = {https://doi.org/10.1016/j.coche.2019.02.009},
    issn = {2211-3398},
    journal = {Current Opinion in Chemical Engineering},
    month = {jan},
    pages = {51--57},
    title = {Advances of machine learning in molecular modeling and simulation},
    volume = {23},
    year = {2019}
    }

    @article{Hachmann2018,
    author = {Hachmann, Johannes and Afzal, Mohammad Atif Faiz and Haghighatlari, Mojtaba and Pal, Yudhajit},
    doi = {10.1080/08927022.2018.1471692},
    issn = {10290435},
    journal = {Molecular Simulation},
    number = {11},
    pages = {921--929},
    title = {Building and deploying a cyberinfrastructure for the data-driven design of chemical systems and the exploration of chemical space},
    volume = {44},
    year = {2018}
    }


.. toctree::
   :maxdepth: 2
   :caption: ChemML Wrapper documentation

   CMLWTutorial
   CMLWInputFile
   CMLWInputFileGenerator
   CMLWContentsTable
   CMLWReference

.. toctree::
   :maxdepth: 2
   :caption: ChemML library Tutorial

   Molecule.ipynb
   active_model_based.ipynb
   ga_hyper_opt.ipynb
   ga_feature_selection.ipynb

..   tutorial.chem
..   tutorial.optimization


.. toctree::
   :maxdepth: 2
   :caption: ChemML library documentation

   chemml.chem
   chemml.chem.magpie_python
   chemml.initialization
   chemml.datasets
   chemml.preprocessing
   chemml.models
   chemml.optimization
   chemml.visualization




License:
++++++++
ChemML is copyright (C) 2014-2018 Johannes Hachmann and Mojtaba Haghighatlari, all rights reserved.
ChemML is distributed under 3-Clause BSD License (https://opensource.org/licenses/BSD-3-Clause).


About us:
++++++++

:Maintainers:
    - Johannes Hachmann, hachmann@buffalo.edu
    - Mojtaba Haghighatlari
    University at Buffalo - The State University of New York (UB)

:Contributors:
    - Doaa Altarawy (MolSSI): scientific advice and software mentor
    - Gaurav Vishwakarma (UB): automated model optimization
    - Ramachandran Subramanian (UB): Magpie descriptor library port
    - Bhargava Urala Kota (UB): library database
    - Aditya Sonpal (UB): debugging
    - Srirangaraj Setlur (UB): scientific advice
    - Venugopal Govindaraju (UB): scientific advice
    - Krishna Rajan (UB): scientific advice

    - We encourage any contributions and feedback. Feel free to fork and make pull-request to the "development" branch.

:Acknowledgements:
    - ChemML is based upon work supported by the U.S. National Science Foundation under grant #OAC-1751161 and in part by #OAC-1640867.
    - ChemML was also supported by start-up funds provided by UB's School of Engineering and Applied Science and UB's Department of Chemical and Biological Engineering, the New York State Center of Excellence in Materials Informatics through seed grant #1140384-8-75163, and the U.S. Department of Energy under grant #DE-SC0017193.
    - Mojtaba Haghighatlari received 2018 Phase-I and 2019 Phase-II Software Fellowships by the Molecular Sciences Software Institute (MolSSI) for his work on ChemML.


.. |logo| image:: images/logo.png
   :width: 540 px
   :target: https://mojtabah.github.io/ChemML
