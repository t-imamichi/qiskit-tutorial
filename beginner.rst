.. image:: images/QISKit-c.gif
    :align: center

Beginner's guide for installation and setup
-------------------------------------------


1. Get the tutorials and install the QISKit SDK
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


1. install `conda <https://conda.io/docs/index.html>`_
2. get the tutorials

.. code:: sh

    git clone https://github.com/QISKit/qiskit-tutorial.git

2. create conda environment for QISKit and install packages

.. code:: sh

    cd qiskit-tutorial
    conda create env -f qiskit-simple.yml

3. activate the environment

   - MacOS, Linux: ``source activate QISKitenv``
   - Windows: ``activate QISKitenv``

4. setup API token

    1. Create an
       `IBM Quantum Experience Experience <https://quantumexperience.ng.bluemix.net>`__
       account if you haven't already done so
    2. Get an API token from the Quantum Experience website under "My Account" > "Personal Access Token"
    3. You will set your API token in the environment variable ``IBMQE_API``

        - MacOS, Linux (bash): ``export IBMQE_API=(your token)``
        - Windows: ``SETX IBMQE_API "(your token)"``

    Reference of ``SETX``: https://docs.microsoft.com/en-us/windows-server/administration/windows-commands/setx


2. Explore the tutorials
~~~~~~~~~~~~~~~~~~~~~~~~

Start Jupyter with the index notebook.

.. code:: sh

    jupyter notebook index.ipynb

