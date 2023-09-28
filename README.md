# econo-python: An Interbank ABM model used during the classes

- Auxiliary files:
  - *requirements.txt*: list of the necessary python packages


## - Interbank model

  - *interbank.py*: use to execute standalone the Interbank simulation.
    - It accepts command line options. For instance, you can execute this:
    
          interbank.py --log DEBUG --n 150 --t 2000
    - When it is used as a package, the sequence should be:

          import interbank
          model = interbank.Model()
          model.configure( param=x )
          model.forward()
          μ = model.get_current_fitness()
          model.set_policy_recommendation( ŋ=0.5 )


  - *interbank.ipynb*: Notebook version of the standalone *interbank.py* with the same results but plotted using Bokeh.
  - *interbank.lml*: LabPlot2 file to plot the results of the *interbank.py*.



