# 3D-Ken-Burns-effect-fixxed-working
3D-Ken-Burns effect fixxed/working colab

You can run this project via browser through the following google colab link: https://colab.research.google.com/github/400lbhacker/3D-Ken-Burns-effect-fixxed-working/blob/main/3D_Ken_Burns_fixxed.ipynb

Made over 20 error repairs. to much to indivudally add but involved fixxing multiple broken refrences, removing redundencies(makes it alot faster) and complimentary compressing the code modules to make the entire process from start to finish much more straight to the point.

To customize the effects. You want to browser to the following file located within the directory: /content/3d-ken-burns/autozoom.py 
and play with the values within the following lines (towards bottom of file) 

objectTo = process_autozoom({
'dblShift': 10.0,
'dblZoom': 10000000000000000000000000000000000000000000000000000000,
'objectFrom': objectFrom
})
numpyResult = process_kenburns
({'dblSteps': numpy.linspace(0.0, 8.0, 400).tolist(),
'objectFrom': objectFrom,
'objectTo': objectTo,
'boolInpaint': True
})

I found this code located here but was difficult to get working, credits to original author though:
https://towardsdatascience.com/12-colab-notebooks-that-matter-e14ce1e3bdd0
