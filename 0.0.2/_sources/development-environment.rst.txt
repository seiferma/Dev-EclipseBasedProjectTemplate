Development Environment
=======================

The development depends on what you want to do. 


Minimum Requirements for Building
---------------------------------

To only build the resulting project, you have to have the following things installed:

* Java > 11
* Maven > 3.6.2

No special configuration of the tools is required. If you have multiple Java versions installed and the default version is not compatible with the version above, ensure to set the ``JAVA_HOME`` variable is set to the compatible version before launching Maven.


Requirements for Developing in Eclipse
--------------------------------------

We assume that you are using the Eclipse IDE for development purposes because other IDEs struggle with using Eclipse update sites. Before staring, you have to do the steps described in :ref:`Minimum Requirements for Building`.

Download the  `Eclipse Modeling Edition <https://www.eclipse.org/downloads/packages/>`_ in a recent version. The modeling edition provides best compatibility with our development workflow. The minimum required version depends on the parent POM used in the root ``pom.xml`` file. For the version used in this repository, you have to use ``2019-09`` at least.

.. todo:: There is no description about how to determine the required Eclipse version yet. This has to be added to the documentation.

Install all dependencies included by the build scripts. Again, this dependens on the used parent POM. It is usually safe to install all dependencies described in the latest target platform of our correpsonding `Github repository <https://github.com/MDSD-Tools/Maven-Build-TargetPlatforms/tree/master/targetPlatforms>`_.

.. todo:: There is no description about how to determine the required features yet. This has to be added to the documentation.


Requirements of Specific Project
--------------------------------

This project has no additional dependencies but others might have. Please refer to :ref:`dev-eclipse-build` for information where to find additional project dependencies.