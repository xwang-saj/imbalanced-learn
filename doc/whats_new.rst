.. currentmodule:: imbalanced-learn

===============
Release history
===============

.. _changes_0_2:

Version 0.2
===========

Changelog
---------

New features
~~~~~~~~~~~~

- Added AllKNN under sampling technique.

API changes summary
~~~~~~~~~~~~~~~~~~~

- Two base classes :class:`BaseBinaryclassSampler` and :class:`BaseMulticlassSampler` have been created to handle the target type and raise warning in case of abnormality.

Enhancement
~~~~~~~~~~~

- Added support for bumpversion.
- Validate the type of target in binary samplers. A warning is raised for the moment.

Documentation changes
~~~~~~~~~~~~~~~~~~~~~

- Added doctest in the documentation.

.. _changes_0_1:

Version 0.1
===========

Changelog
---------

API
~~~

- In :class:`ensemble.EasyEnsemble`, correction of the `random_state` generation.
- First release of the stable API.

New methods
~~~~~~~~~~~

* Under-sampling
    1. Random majority under-sampling with replacement
    2. Extraction of majority-minority Tomek links
    3. Under-sampling with Cluster Centroids
    4. NearMiss-(1 & 2 & 3)
    5. Condensend Nearest Neighbour
    6. One-Sided Selection
    7. Neighboorhood Cleaning Rule
    8. Edited Nearest Neighbours
    9. Instance Hardness Threshold
    10. Repeated Edited Nearest Neighbours

* Over-sampling
    1. Random minority over-sampling with replacement
    2. SMOTE - Synthetic Minority Over-sampling Technique
    3. bSMOTE(1 & 2) - Borderline SMOTE of types 1 and 2
    4. SVM SMOTE - Support Vectors SMOTE
    5. ADASYN - Adaptive synthetic sampling approach for imbalanced learning

* Over-sampling followed by under-sampling
    1. SMOTE + Tomek links
    2. SMOTE + ENN

* Ensemble sampling
    1. EasyEnsemble
    2. BalanceCascade
