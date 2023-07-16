Loading results from pickles
============================

To load results, you can use the :mod:`scsr.results` module:
    
.. code-block:: python

    >>> from scsr.results import load_results
    >>> load_results(["../test.pkl"])
    Loading ../test.pkl
    <EpsilonResults: steps=150 L=50 tau=10 P=0, Kx=0.001:0.4:4>

This will return a :class:`Results` instance with which you can inspect the data.

unrelated maths:
----------------


    
    The **characteristic polynomial** :math:`\chi(\lambda)` of the
    :math:`3 \times 3` matrix:

.. math::
    
    M = \begin{bmatrix}
        a & b & c \\
        d & e & f \\
        g & h & i
        \end{bmatrix}
    
is given by the formula

.. math::

    \chi(\lambda) = \begin{bmatrix}
                    \lambda - a & -b & -c \\
                    -d & \lambda - e & -f \\
                    -g & -h & \lambda - i 
                    \end{bmatrix}