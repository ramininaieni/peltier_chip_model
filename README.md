# peltier_chip_model
This repository includes code in Julia that can be used to model the behavior of any Peltier chip well, given twenty experimental data points that are often provided by Peltier chip manufacturers. To easily take users through the code, it is in the format of a Jupyter notebook.
<h2> Ubuntu Installation Instructions</h2>
<h3>Setting up Julia</h3>
If you don't have Julia, in terminal run <code>sudo-apt install Julia</code>. This method works for running my code, but others recommend a more foolproof method of installation detailed here: https://medium.com/coffee-in-a-klein-bottle/install-julia-1-5-on-ubuntu-bb8be4b2571d

Type <code>julia</code> in the terminal, then run <code>import Pkg; Pkg.add("Plots")</code>. After, run <code>import Pkg; Pkg.add("Optim")</code>. 
<h3>Setting up Jupyter Notebook</h3>
I always recommend using a conda environment past this step, but it is not necessary. Ensure your conda environmnet has Python 3.8+. In your conda environment, run <code>pip install notebook</code>
<h3>Running Code</h3>
In your conda environment, run <code>jupyter-notebook</code> and navigate to the <code>peltier_chip_model.ipynb</code> file. Follow the instructions on the page and click each code block and hold the <code>shift</code> key and then hit the <code>enter</code> key to run each block. This should convert the number in the top left of each code block into an asterisk. Wait until the asterisk converts back to a number, indicating that the block is done running, until running another block. All blocks should be run in order, top down. 
<h2>Power of Model</h2>
Here are some graphs depicting how well my model predicted the behavior of some of <a href = "https://tetech.com/peltier-thermoelectric-cooler-modules/standard/" target = "_blank">TE Tech's Peltier Chips</a>
<h4>HP-127-1.0-1.3-71 Thermoelectric Module</h4>
<img src = "https://github.com/ramininaieni/peltier_chip_model/blob/main/Media/cop_first_chip.png">
<img src = "https://github.com/ramininaieni/peltier_chip_model/blob/main/Media/currents_first_chip.png">
<img src = "https://github.com/ramininaieni/peltier_chip_model/blob/main/Media/heats_pumped_first_chip.png">
<h4>TE-71-1.0-2.0 Thermoelectric Module</h4>
<img src = "https://github.com/ramininaieni/peltier_chip_model/blob/main/Media/cop_second_chip.png">
<img src = "https://github.com/ramininaieni/peltier_chip_model/blob/main/Media/currents_second_chip.png">
<img src = "https://github.com/ramininaieni/peltier_chip_model/blob/main/Media/heats_pumped_second_chip.png">
