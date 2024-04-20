# Comparing `tmp/auto_vtna-1.0.1.tar.gz` & `tmp/auto_vtna-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_vtna-1.0.1.tar", last modified: Fri Apr 19 11:29:36 2024, max compression
+gzip compressed data, was "auto_vtna-1.0.2.tar", last modified: Sat Apr 20 16:05:52 2024, max compression
```

## Comparing `auto_vtna-1.0.1.tar` & `auto_vtna-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 11:29:36.163051 auto_vtna-1.0.1/
--rw-rw-rw-   0        0        0      539 2024-04-19 11:29:36.162050 auto_vtna-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      274 2024-04-18 14:11:13.000000 auto_vtna-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 11:29:36.137359 auto_vtna-1.0.1/auto_vtna/
--rw-rw-rw-   0        0        0   139688 2024-04-19 11:26:22.000000 auto_vtna-1.0.1/auto_vtna/Auto_VTNA_GUI.py
--rw-rw-rw-   0        0        0    22228 2024-04-18 20:28:15.000000 auto_vtna-1.0.1/auto_vtna/Automatic_VTNA.py
--rw-rw-rw-   0        0        0    23125 2024-04-18 20:28:15.000000 auto_vtna-1.0.1/auto_vtna/Normal_VTNA.py
--rw-rw-rw-   0        0        0    44993 2024-04-18 20:28:15.000000 auto_vtna-1.0.1/auto_vtna/VTNA_functions.py
--rw-rw-rw-   0        0        0    48521 2024-04-19 11:25:57.000000 auto_vtna-1.0.1/auto_vtna/__init__.py
--rw-rw-rw-   0        0        0     2813 2024-04-19 11:24:17.000000 auto_vtna-1.0.1/auto_vtna/running_codes 23dec.py
-drwxrwxrwx   0        0        0        0 2024-04-19 11:29:36.159043 auto_vtna-1.0.1/auto_vtna.egg-info/
--rw-rw-rw-   0        0        0      539 2024-04-19 11:29:35.000000 auto_vtna-1.0.1/auto_vtna.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      345 2024-04-19 11:29:35.000000 auto_vtna-1.0.1/auto_vtna.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 11:29:35.000000 auto_vtna-1.0.1/auto_vtna.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2024-04-19 11:29:35.000000 auto_vtna-1.0.1/auto_vtna.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-19 11:29:35.000000 auto_vtna-1.0.1/auto_vtna.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-19 11:29:36.164054 auto_vtna-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      929 2024-04-19 11:29:24.000000 auto_vtna-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 16:05:52.677625 auto_vtna-1.0.2/
+-rw-rw-rw-   0        0        0      539 2024-04-20 16:05:52.676535 auto_vtna-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2024-04-18 14:11:13.000000 auto_vtna-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-20 16:05:52.655546 auto_vtna-1.0.2/auto_vtna/
+-rw-rw-rw-   0        0        0   139857 2024-04-20 15:39:25.000000 auto_vtna-1.0.2/auto_vtna/Auto_VTNA_GUI.py
+-rw-rw-rw-   0        0        0    22228 2024-04-18 20:28:15.000000 auto_vtna-1.0.2/auto_vtna/Automatic_VTNA.py
+-rw-rw-rw-   0        0        0    23125 2024-04-18 20:28:15.000000 auto_vtna-1.0.2/auto_vtna/Normal_VTNA.py
+-rw-rw-rw-   0        0        0    45282 2024-04-20 15:02:10.000000 auto_vtna-1.0.2/auto_vtna/VTNA_functions.py
+-rw-rw-rw-   0        0        0    50480 2024-04-20 15:38:27.000000 auto_vtna-1.0.2/auto_vtna/__init__.py
+-rw-rw-rw-   0        0        0     3110 2024-04-20 15:39:25.000000 auto_vtna-1.0.2/auto_vtna/running_codes 23dec.py
+drwxrwxrwx   0        0        0        0 2024-04-20 16:05:52.673532 auto_vtna-1.0.2/auto_vtna.egg-info/
+-rw-rw-rw-   0        0        0      539 2024-04-20 16:05:51.000000 auto_vtna-1.0.2/auto_vtna.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      345 2024-04-20 16:05:52.000000 auto_vtna-1.0.2/auto_vtna.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 16:05:51.000000 auto_vtna-1.0.2/auto_vtna.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2024-04-20 16:05:51.000000 auto_vtna-1.0.2/auto_vtna.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-20 16:05:51.000000 auto_vtna-1.0.2/auto_vtna.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-20 16:05:52.677625 auto_vtna-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      963 2024-04-20 15:01:17.000000 auto_vtna-1.0.2/setup.py
```

### Comparing `auto_vtna-1.0.1/PKG-INFO` & `auto_vtna-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto_vtna
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python package for efficient and automatic VTNA analysis
 Author: Daniel Dalland
 Author-email: dd4518@ic.ac.uk
 License: MIT
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
```

### Comparing `auto_vtna-1.0.1/auto_vtna/Auto_VTNA_GUI.py` & `auto_vtna-1.0.2/auto_vtna/Auto_VTNA_GUI.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 import PySimpleGUI as sg
 import threading
 import pandas as pd
 import numpy as np
 import matplotlib
-#matplotlib.use('Qt5Agg')
-matplotlib.use('TkAgg')
+matplotlib.use('Qt5Agg')
 import matplotlib.pyplot as plt
 import auto_vtna
 import tkinter as tk
 from auto_vtna.Normal_VTNA import Normal_VTNA
 from auto_vtna.VTNA_functions import VTNA_omissions
 from auto_vtna.Automatic_VTNA import Automatic_VTNA
-import openpyxl.cell._writer
 import copy
 import re
 import csv
 import tkinter as tk
 from tkinter import scrolledtext
 
 def extract_range_info(values,data):
@@ -98,29 +96,29 @@
     converted to a float without giving an error.'''
     try:
         float_value = float(string)
         return True
     except ValueError:
         return False
 
-def overlay_plot(kinetic_data,sheets,NS_dict,output_reaction_species,tt_scaler=1,y_unit='M',\
+def overlay_plot(kinetic_data,experiments,NS_dict,output_reaction_species,tt_scaler=1,y_unit='M',\
                  size_scaler=1,grid=False,title=None,fit_metric='RMSE',constraint='monotonic',\
                  deg=5,show_fit_function=False,show_overlay_score=False,DP_scaler=1,xtick_rotation=0,\
                  show_legend=True,legend_outside=False,extra_legend=True,line_scaler=1,
                  tT_notation='Normal'):
     ''' Creates a VTNA_selection dictionary for the GUI settings stored in the arguments
-    "sheets", "NS_dict" and "output_reaction_species", calculates the transformed time axis 
+    "experiments", "NS_dict" and "output_reaction_species", calculates the transformed time axis 
     for the kinetic data "kinetic_data" and generates the overlay plot for the selected plot settings.
     '''
     # Generate a VTNA selection dictionary template.
     Default_VTNA_selection_dictionary=auto_vtna.make_VTNA_selection(kinetic_data)
     VTNA_selection_dictionary={}
     # Generate a sub-dictionary to specify which experiments to include based on sheet selections.
     VTNA_selection_dictionary['RM']={}
-    for i in sheets:
+    for i in experiments:
         VTNA_selection_dictionary['RM'][i]=Default_VTNA_selection_dictionary['RM'][i]
     # Update the normalised species and output species for generating the overlay plot based on GUI selections.
     VTNA_selection_dictionary['normalised_species']=NS_dict
     VTNA_selection_dictionary['output_species']=output_reaction_species
     # Calculate the normalised time axis using Normal_VTNA from auto_vtna.
     Run_VTNA=Normal_VTNA(kinetic_data,VTNA_selection_dictionary)
     if constraint=='through origin':
@@ -218,26 +216,26 @@
     "Checks if a variable can be converted to an integer."
     try:
         int(value)
         return True
     except ValueError:
         return False
 
-def run_calculation(data, selected_sheets,selected_columns, selected_result_columns, calculation_settings):
+def run_calculation(data, selected_experiments,selected_columns, selected_result_columns, calculation_settings):
     '''Runs calculation by preparing the applied calculation settings to be inputted into 
     Auto-VTNA.'''
     # Create a VTNA selection dictonary.
     VTNA_selection_dict=auto_vtna.make_VTNA_selection(data)
     # Add the normalised species selected in the GUI with orders of 1 as placeholders.
     VTNA_selection_dict['normalised_species']={}
     for molecule in selected_columns:
         VTNA_selection_dict['normalised_species'][molecule]=1
     # Define the experiments selected in the GUI that will be included in the calculation.
     VTNA_selection_dict['RM']={}
-    for i in selected_sheets:
+    for i in selected_experiments:
         VTNA_selection_dict['RM'][i]={}
         VTNA_selection_dict['RM'][i]["omissions"]=None
     # Define the output species specified in the GUI.
     VTNA_selection_dict['output_species']=selected_result_columns[0]
     # Define the fixed order species with their selected order values. 
     fixed_order_species=calculation_settings["fixed_order_species"]
     if fixed_order_species!=None:
@@ -419,28 +417,28 @@
     # Define other miscellaneous placeholders.
     best_order_dict={}
     best_order_dict_rounded={}
     omission_dictionary=None
     omission_range_dictionary={}
     omission_range_dictionary["range_type"]='Percentage'
     omission_mode='Datapoint mode'
-    Plot_concentration_profiles_selected_sheets=False
+    Plot_concentration_profiles_selected_experiments=False
     # Define the layout of the main GUI window.
     layout = [
         [sg.Frame("Load Kinetic Data", layout=[
             [sg.Text("Use Excel File:"),
             sg.InputText(key="file_path", enable_events=True, size=(12, 1)), 
             sg.FileBrowse(),sg.Text("Or:"),sg.Button("Use CSVs",key="Select CSVs")]
         ])],
         [sg.Button("Check Data",key="Check Kinetic Data", disabled=True),
          sg.Button("Visualise Data",key="Inspect Kinetic Data", disabled=True),
          sg.Button("Crop Data", key="Crop Kinetic Data", disabled=True),
          sg.Combo(['Range mode', 'Datapoint mode'], default_value=omission_mode,key="crop_mode", enable_events=True, readonly=True,size=(12,1))],
-        [sg.Frame("Select Sheets", layout=[
-            [sg.Listbox(values=[], select_mode=sg.LISTBOX_SELECT_MODE_MULTIPLE, size=(22, 5), key="sheets")]
+        [sg.Frame("Select experiments", layout=[
+            [sg.Listbox(values=[], select_mode=sg.LISTBOX_SELECT_MODE_MULTIPLE, size=(22, 5), key="experiments")]
         ]),
         sg.Frame("Select Normalised Species", layout=[
             [sg.Listbox(values=[], select_mode=sg.LISTBOX_SELECT_MODE_MULTIPLE, size=(21, 5), key="columns")]
         ])],
         [sg.Frame("Select output species", layout=[
             [sg.Listbox(values=[], select_mode=sg.LISTBOX_SELECT_MODE_SINGLE, size=(20, 1), key="result_columns")]
         ]),
@@ -477,15 +475,15 @@
     plt.close()
     # Maintain an infinite loop to process events until the window is shut down
     while True:
         event, values = window.read()
         if event == sg.WIN_CLOSED:
             break
         elif event == "file_path":
-            # Update the list of sheets when a file is selected
+            # Update the list of experiments when a file is selected
             file_path = values["file_path"]
             files_calculation=file_path
             if file_path:
                 try:
                     # Load the kinetic data as a dictionary of Pandas Dataframe objects. 
                     kinetic_data = pd.read_excel(file_path, sheet_name=None)
                     # Reset the best order dictionary and the saved order values for the overlay plot settings. 
@@ -509,19 +507,19 @@
                         omission_mode='Range mode'
                     else:
                         omission_mode='Datapoint mode'
                     # Update the "crop_mode" value. 
                     window["crop_mode"].update(value=omission_mode)
                     # Obtain information from the dataset. 
                     time_label=list(data.values())[0].columns[0]
-                    sheets = list(data.keys())
-                    columns = data[sheets[0]].columns[1:].tolist()  # Exclude the first column
-                    fixed_order_species = data[sheets[0]].columns[1:].tolist()  # All reaction species
+                    experiments = list(data.keys())
+                    columns = data[experiments[0]].columns[1:].tolist()  # Exclude the first column
+                    fixed_order_species = data[experiments[0]].columns[1:].tolist()  # All reaction species
                     # Update the window to add information from the selected kinetic dataset and enable buttons for analysis.
-                    window["sheets"].update(values=sheets)
+                    window["experiments"].update(values=experiments)
                     window["columns"].update(values=columns)
                     window["result_columns"].update(values=columns)
                     window["Run Auto VTNA"].update(disabled=False)  # Enable the "Run Automatic VTNA" button
                     window["calculation_settings"].update(disabled=False)  # Enable the "Calculation Settings" button
                     window["Check Kinetic Data"].update(disabled=False)
                     window["Inspect Kinetic Data"].update(disabled=False)
                     window["Generate Overlay Plot"].update(disabled=False)
@@ -639,15 +637,15 @@
                             sg.popup_error(f"Filename permission error (close excel file with same name): {e}")
                             continue
                     window_save.close()
                     break
 
         elif event == "Run Auto VTNA":
             # Get selected sheet, columns, and result columns
-            selected_sheet = values["sheets"]
+            selected_sheet = values["experiments"]
             selected_columns = values["columns"]
             selected_result_columns = values["result_columns"]
             if selected_sheet and selected_columns and selected_result_columns:
                 # Check that the number of fixed order species is lower than the total number of selected normalised species. 
                 count=len(selected_columns)
                 if type(calculation_settings["fixed_order_species"])==dict:
                     # Raise an error if any fixed order species are not selected as normalised species. 
@@ -710,15 +708,15 @@
                             window['interval_table'].update(values=table_values)
                             window["Overlay Score"].update(overlay_score_string)
                             window["interval_score"].update(calculation_settings['score_interval']*100)
                             window['interval_table'].update(num_rows=len(table_values))   
                 else:
                     sg.popup_error("The number of fixed order species can't be the same as or higher than the number of normalised reaction species.")
             else:
-                sg.popup_error("Please select sheets, reaction species, and output reaction species to run automatic VTNA.")
+                sg.popup_error("Please select experiments, reaction species, and output reaction species to run automatic VTNA.")
         elif event == "refresh_interval_table":
             print(values['interval_score'])
             try:
                 interval_score=values['interval_score']
                 if not is_float(interval_score):
                     raise ValueError("Invalid score interval. Must be numerical")
                 if not float(interval_score)>0:
@@ -1027,17 +1025,17 @@
             except ValueError as e:
                 sg.popup_error(f"Invalid input: {e}")
                 continue
         
         elif event == "Generate Overlay Plot":
             # Ensure that all exisiting plots are closed to avoid bugs.
             plt.close('all')
-            # Define the selected sheets, selected columns and selected output species
+            # Define the selected experiments, selected columns and selected output species
             # for generating the correct VTNA overlay plot. 
-            selected_sheet = values["sheets"]
+            selected_sheet = values["experiments"]
             selected_columns = values["columns"]
             selected_result_columns = values["result_columns"]
             # Define keyword arguments from the overlay_plot_settings dictionary. 
             tt_scaler=overlay_plot_settings['tt_scaler']
             DP_scaler=float(overlay_plot_settings["DP_scaler"])
             line_scaler=float(overlay_plot_settings["line_scaler"])
             xtick_rotation=float(overlay_plot_settings["xtick_rotation"])
@@ -1144,15 +1142,15 @@
                                 overlay_plot(data,selected_sheet,order_values,selected_result_columns[0],tt_scaler=tt_scaler,\
                                          grid=grid,y_unit=y_unit,size_scaler=size_scaler,title=title, fit_metric=fit_metric,
                                          deg=deg,constraint=constraint,show_overlay_score=show_overlay_score,\
                                          show_fit_function=show_fit_function,DP_scaler=DP_scaler,xtick_rotation=xtick_rotation,\
                                          show_legend=legend_bol,legend_outside=legend_outside,extra_legend=extra_legend,\
                                          line_scaler=line_scaler,tT_notation=tT_notation)
             else:
-                sg.popup_error("Please select sheets, reaction species, and output reaction species before generating overlay plot.")
+                sg.popup_error("Please select experiments, reaction species, and output reaction species before generating overlay plot.")
 
         elif event == "calculation_settings":
             # Create the layout for fixed order species based on the pre-existing fixed order species 
             # dictionary in the calculation settings dictionary. 
             fixed_orders={}
             layout_fixed_order=[]
             label_width = max(len(str(compound)) for compound in fixed_order_species)
@@ -1381,22 +1379,22 @@
                     df_nrows=[]
                     for i in kinetic_data.keys():
                         df_nrows.append(kinetic_data[i].shape[0])
                     if max(df_nrows)>25:
                         omission_mode='Range mode'
                     else:
                         omission_mode='Datapoint mode'
-                    # Update the time label and the sheets, column and fixed order species. 
+                    # Update the time label and the experiments, column and fixed order species. 
                     time_label=list(data.values())[0].columns[0]
-                    sheets = list(data.keys())
-                    columns = data[sheets[0]].columns[1:].tolist()  # Exclude the first column
-                    fixed_order_species = data[sheets[0]].columns[1:].tolist()  # All reaction species
+                    experiments = list(data.keys())
+                    columns = data[experiments[0]].columns[1:].tolist()  # Exclude the first column
+                    fixed_order_species = data[experiments[0]].columns[1:].tolist()  # All reaction species
                     # Update the sheet, columns and result column listboxes with the relevant data
                     # (Sheet names, reactant names and reactant names respectively)
-                    window["sheets"].update(values=sheets)
+                    window["experiments"].update(values=experiments)
                     window["columns"].update(values=columns)
                     window["result_columns"].update(values=columns)
                     # Enable various buttons now that the kinetic data has been loaded. 
                     window["Run Auto VTNA"].update(disabled=False)  
                     window["calculation_settings"].update(disabled=False)  
                     window["Check Kinetic Data"].update(disabled=False) 
                     window["Inspect Kinetic Data"].update(disabled=False)
@@ -1665,15 +1663,15 @@
             # Ensure that all exisiting plots are closed to avoid bugs.
             plt.close('all')
             # Define the layout of the window including both buttons for different plots and 
             # the plot settings. 
             layout_inspect_kinetic_data = [
                 [sg.Button("Generate Initial Concentration Table")],
                 [sg.Button("Plot Kinetic Data")],
-                [sg.Button("Plot Kinetic Data for Selected Sheets and Species")],
+                [sg.Button("Plot Kinetic Data for Selected Experiments and Species")],
                 [sg.Button("Plot Concentration Profiles")],
                 [sg.Frame("Settings", layout=[
                     [sg.Text("Concentration unit:"),
                      sg.InputText(key="y_unit", size=(5, 1),default_text=str(data_plotting_settings["y_unit"])),
                      sg.Text("Time unit:"),
                      sg.InputText(key="t_unit", size=(5, 1),default_text=str(data_plotting_settings["t_unit"]))],
                     [sg.Text("Figure size scaler:"),
@@ -1698,20 +1696,23 @@
             # Maintain an infinite loop to process events until the window is shut down.
             while True:
                 event_inspect_kinetic_data, values_inspect_kinetic_data = window_inspect_kinetic_data.read()
                 if event_inspect_kinetic_data == sg.WIN_CLOSED or event_inspect_kinetic_data == "Back":
                     break
                 # Check that the inputed settings are valid before creating any plots or table. 
                 if event_inspect_kinetic_data in ["Generate Initial Concentration Table","Plot Kinetic Data",
-                        "Plot Kinetic Data for Selected Sheets and Species","Plot Concentration Profiles"]:
+                        "Plot Kinetic Data for Selected Experiments and Species","Plot Concentration Profiles"]:
                     try:
                         if not is_float(values_inspect_kinetic_data["ylim"]):
                             ylim = None
                         else: 
                             ylim = float(values_inspect_kinetic_data["ylim"])
+                        if event_inspect_kinetic_data=="Plot Kinetic Data for Selected Experiments and Species":
+                            print(values['columns'])
+                            print(values["experiments"])
                         y_unit = values_inspect_kinetic_data["y_unit"]
                         t_unit = values_inspect_kinetic_data["t_unit"]
                         if not is_float(values_inspect_kinetic_data["SF"]):
                             raise ValueError("Significant figures for initial concentration table must be a numerical value.")
                         significant_figures=int(abs(float(values_inspect_kinetic_data["SF"])))
                         data_plotting_settings["legend_position"]=values_inspect_kinetic_data["legend_position"]
                         DP_scaler = float(values_inspect_kinetic_data["DP_scaler"])
@@ -1817,30 +1818,30 @@
                                             break
                                     window_stoichiometry_values.close()
                                 break
                         window_select_species.close()
                     else:
                         # If the user chooses not to visualise mass balance, call the plot_kinetic_data function without 
                         plot_kinetic_data(data,None,data_plotting_settings)
-                elif event_inspect_kinetic_data == "Plot Kinetic Data for Selected Sheets and Species":  
-                    # Selected the sheets and reaction species selected by the user. 
-                    selected_sheets = values["sheets"]
+                elif event_inspect_kinetic_data == "Plot Kinetic Data for Selected Experiments and Species":  
+                    # Selected the experiments and reaction species selected by the user. 
+                    selected_experiments = values["experiments"]
                     selected_species = values["columns"]
-                    # Create an error message is no selected sheets or species have been selected. 
-                    if not selected_sheets and not selected_species:
-                        sg.popup_error("No sheets nor reaction species have been selected.\n Kinetic data for every reaction species in every sheet will be plotted.")
+                    # Create an error message is no selected experiments or species have been selected. 
+                    if not selected_experiments and not selected_species:
+                        sg.popup_error("No experiments nor reaction species have been selected.")
+                    elif not selected_experiments:
+                        sg.popup_error("No experiments have been selected.")
+                    elif not selected_species:
+                        sg.popup_error("No reaction species have been selected.")
                     else:
-                        if not selected_species:
-                            sg.popup_error("No reaction species have been selected.\n Kinetic data for every reaction species in the selected sheets will be plotted.")
-                        elif not selected_sheets:
-                            sg.popup_error("No sheets have been selected.\n Kinetic data for the selected reaction species in every sheet will be plotted.")
                         # Create a modified kinetic data variable. First, add the dataframes for each selected sheet.
                         data_2=copy.deepcopy(data)
                         data_modified={}
-                        for exp in selected_sheets:
+                        for exp in selected_experiments:
                             data_modified[exp]=data_2[exp]
                         # Remove the concentration profiles not included in "selected_species" from the kinetic data.
                         for RM in data_modified.keys():
                             for i, NS in enumerate(data_modified[RM]):
                                 if NS not in selected_species and i!=0:
                                     del data_modified[RM][NS]
                         # Ask the user whether to visualise mass balance using a custom popup window. 
@@ -1917,37 +1918,37 @@
                         default_value=reaction_species_list[0] if reaction_species_list else "",
                         size=(20, 1),
                         key="selected_species_dropdown",)
                     # Create the select species layout. 
                     layout_select_species = [
                         [sg.Text("Select one reaction species for concentration profiles:")],
                         [selected_species],
-                        [sg.Checkbox("Only include selected sheets",key='sheets',default=Plot_concentration_profiles_selected_sheets,enable_events=True)],
+                        [sg.Checkbox("Only include selected experiments",key='experiments',default=Plot_concentration_profiles_selected_experiments,enable_events=True)],
                         [sg.Button("OK"), sg.Button("Cancel")]]
                     # Create a window for selecting reaction species. 
                     window_select_species = sg.Window("Select Reaction Species", layout_select_species)
                     # Maintain an infinite loop to process events until the window is shut down.
                     while True:
                         event_select_species, values_select_species = window_select_species.read()
                         if event_select_species == sg.WIN_CLOSED or event_select_species == "Cancel":
                             break
                         elif event_select_species == "OK":
-                            # Define the sheets selected by the user. 
-                            Plot_concentration_profiles_selected_sheets=values_select_species['sheets']
-                            selected_sheets = values["sheets"]
+                            # Define the experiments selected by the user. 
+                            Plot_concentration_profiles_selected_experiments=values_select_species['experiments']
+                            selected_experiments = values["experiments"]
                             # Modify the dataset to only include the concentration profiles of the selected species. 
-                            if Plot_concentration_profiles_selected_sheets and len(selected_sheets)>0:
+                            if Plot_concentration_profiles_selected_experiments and len(selected_experiments)>0:
                                 data_2=copy.deepcopy(data)
                                 data_modified={}
-                                for exp in selected_sheets:
+                                for exp in selected_experiments:
                                     data_modified[exp]=data_2[exp]
                             selected_species_value = values_select_species["selected_species_dropdown"]
                             # Plot the modified kinetic data. 
                             if selected_species_value:
-                                if Plot_concentration_profiles_selected_sheets and len(selected_sheets)>0:
+                                if Plot_concentration_profiles_selected_experiments and len(selected_experiments)>0:
                                     plot_concentration_profiles(data_modified, selected_species_value,data_plotting_settings)
                                 else:
                                     plot_concentration_profiles(data, selected_species_value,data_plotting_settings)
                             break
                     window_select_species.close()
             window_inspect_kinetic_data.close()
     window.close()
```

### Comparing `auto_vtna-1.0.1/auto_vtna/Automatic_VTNA.py` & `auto_vtna-1.0.2/auto_vtna/Automatic_VTNA.py`

 * *Files identical despite different names*

### Comparing `auto_vtna-1.0.1/auto_vtna/Normal_VTNA.py` & `auto_vtna-1.0.2/auto_vtna/Normal_VTNA.py`

 * *Files identical despite different names*

### Comparing `auto_vtna-1.0.1/auto_vtna/VTNA_functions.py` & `auto_vtna-1.0.2/auto_vtna/VTNA_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import numpy as np
 import time
 import pandas as pd
 from polyfit import PolynomRegressor, Constraints
 from num2words import num2words
-from sklearn.metrics import r2_score
-from sklearn.metrics import mean_squared_error
 from scipy.optimize import curve_fit
 import itertools
 import copy
 import matplotlib.pyplot as plt
 import warnings
 
 def VTNA_orders(data,VTNA_selection,order_range=[-1.5,2.5],resolution=8,deg=5,fit_metric='RMSE',iterations=6,constraint='monotonic',
@@ -564,24 +562,30 @@
         if shifted:
             y_label='Shifted '+y_label
         ax2.set_ylabel(y_label)
         plt.title(title_string)
         plt.tight_layout()
         plt.show()
 
-def score_fit(y,y_fit,fit_metric):
+def score_fit(y, y_fit, fit_metric):
+    # NB: this function was written with the help of OpenAI's ChatGTP. 
     # Find the variance of the residuals of the fit
-    FQ=np.var(np.array(y_fit)-np.array(y))
+    FQ = np.var(np.array(y_fit) - np.array(y))
     # Update the goodness-of-fit value according to the chosen fit metric.
-    if fit_metric=='R2':
-        FQ=r2_score(y,y_fit)
-    if fit_metric=='SE':
-        FQ=FQ**0.5/len(y)**0.5
-    if fit_metric=='RMSE':
-        FQ=np.sqrt(mean_squared_error(y_fit,y))
+    if fit_metric == 'R2':
+        # Compute R-squared manually
+        SS_res = np.sum((np.array(y) - np.array(y_fit))**2)
+        SS_tot = np.sum((np.array(y) - np.mean(np.array(y)))**2)
+        FQ = 1 - (SS_res / SS_tot)
+    elif fit_metric == 'SE':
+        # Compute Standard Error of the Estimate
+        FQ = FQ**0.5 / len(y)**0.5
+    elif fit_metric == 'RMSE':
+        # Compute Root Mean Squared Error
+        FQ = np.sqrt(np.mean((np.array(y_fit) - np.array(y))**2))
     return FQ
 
 def VTNA_new(data,VTNA_selection):
     """
     First removes experimental data as specified in "VTNA_selection" from "data". Then \
     calculates the normalised time axis using the trapezoid rule for the concentration \
     profiles of the reaction species listed in "normalised_species" with their respective \
```

### Comparing `auto_vtna-1.0.1/auto_vtna/__init__.py` & `auto_vtna-1.0.2/auto_vtna/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -312,22 +312,20 @@
         y_unit (str, optional): Concentration unit to be included in the Y axis label. 
         t_unit (str, optional): Time unit to be included in the X axis label. 
         fig_size_scaler (float or int, optional): Scaler to adjust the size of the graphs by the \
         selected factor.
         plot_mode (str): Either set to "scrollable" to generate a single graph which updates \
         to the next or previous graph by clicking right or left arrow keys, or 'together' to \
         plot graphs for each experiment together. If plot_mode is set to something else, \
-        graphs will pop-up one after the other.
-        legend_outside (bol): Set to True to ensure that the to place the plot legend to the right \
-        of the plot axis object, or in a separate box if plot_mode=together. Set to False (by default) \
-        to show the legend in the main plot(s)
-        DP_scaler (float or int): Number by which the datapoints are scaled away from the standard size of 6. \
-        Can be set to 0 to remove datapoints all together.  
-        linewidth (float or int): Defines the linewidth of the graphs in the plot. Can be set to 0 to remove \
-        lines all together.  
+        graphs will pop-up one after the other. 
+        legend_outside (bol): Set to False by default to show legend inside the axis of the plot. \
+        Can be set to True to show the legend outside the axis (top right). 
+        DP_scaler (float, int): Factor by which the datapoints of the plots is scaled from a standard \
+        value of 6. 
+        linewidth (float, int): The linewidth parameter used to generate plots. Is by default set to 1. 
     """
     # Set the datapoint size scaler to 1 if an incorrect value has been assigned.
     if DP_scaler==None or isinstance(DP_scaler, str):
         DP_scaler=1
     if plot_mode=='together':
         addition=0
         if legend_outside:
@@ -379,21 +377,22 @@
             ax.spines['bottom'].set_visible(False)
             ax.set_xticklabels([])
             ax.set_yticklabels([])
             ax.set_xticks([])
             ax.set_yticks([])
             ax.legend(handles, labels, loc='center')
         # Remove empty subplots if there are any
-        for i in range(len(data)+addition, num_cols * num_rows):
+        for i in range(len(data)+1, num_cols * num_rows):
             fig.delaxes(axs.flatten()[i])
         plt.show()
     elif plot_mode=='scrollable':
         # Define a class for creating scrollable plots
         class ScrollablePlot:
-            def __init__(self, data_dict, ylim=None, y_unit='M', t_unit=None, fig_size_scaler=1,legend_outside=legend_outside,DP_scaler=1,linewidth=linewidth):
+            def __init__(self, data_dict, ylim=None, y_unit='M', t_unit=None, 
+                         fig_size_scaler=1,legend_outside=legend_outside,DP_scaler=1,linewidth=1):
                 # Extract data and labels from the given dictionary
                 data_1 = [data_dict[i] for i, j in data_dict.items()]
                 data_labels = list(data_dict.keys())
                 # Initialize instance variables
                 self.data = data_1
                 self.labels = data_labels
                 self.current_plot_index = 0
@@ -404,15 +403,15 @@
                 self.legend_outside=legend_outside
                 self.DP_scaler=DP_scaler
                 self.linewidth=linewidth
                 # Create a Matplotlib figure and axis
                 self.fig, self.ax = plt.subplots()
                 # Create a note to inform user of scrolling feature.
                 note_text = 'NB: Use left or right arrows to scroll to other experiments.'
-                self.fig.text(0.5, -0.05, note_text, ha='center', color='gray')
+                self.fig.text(0.5, 0.015, note_text, ha='center', color='gray')
                 # Plot the initial data
                 self.plot_current_data()
                 # Enable hovering using mplcursors
                 mplcursors.cursor(hover=True)
                 # Connect the key press event to the corresponding method
                 self.fig.canvas.mpl_connect('key_press_event', self.on_key_press)
 
@@ -425,15 +424,16 @@
                 # Extract time and concentration data
                 t = current_data.columns[0]
                 time_column = current_data[t]
                 # Plot each concentration profile
                 for i in current_data.keys():
                     if i == t:
                         continue
-                    self.ax.plot(time_column, current_data[i], label=i, marker='o',markersize=6*self.DP_scaler,linewidth=self.linewidth)
+                    self.ax.plot(time_column, current_data[i], label=i, marker='o',
+                                 markersize=6*self.DP_scaler,linewidth=self.linewidth)
                 # Set the figure size
                 self.fig.set_size_inches(7 *0.8* self.fig_size_scaler, 5 *0.8* self.fig_size_scaler)
                 # Set plot title
                 self.ax.set_title(f'Concentration profiles in {current_label}')
                 # Set x-axis label
                 if self.t_unit is not None:
                     self.ax.set_xlabel(f'Time / {self.t_unit}')
@@ -442,15 +442,32 @@
                 # Set y-axis label
                 self.ax.set_ylabel(f'Concentration / {self.y_unit}')
                 # Set y-axis limit if specified
                 if self.ylim is not None and isinstance(self.ylim, (float, int)):
                     self.ax.set_ylim(0, self.ylim)
                 # Display legend
                 if self.legend_outside:
-                    self.ax.legend(bbox_to_anchor=(1, 0.78))
+                    # Calculate the width of the legend dynamically based on the longest text element
+                    legend = self.ax.legend()
+                    # Obtain the legend width in display units. 
+                    legend_bbox = legend.get_window_extent()
+                    legend_width = legend_bbox.width
+                    # Obtain the figure width in display units.
+                    fig_box = plt.gcf().get_window_extent()
+                    fig_width_display = fig_box.width
+                    # See by what fraction the figure width needs to be extended for outside legend.
+                    legend_width_scaled=legend_width/fig_width_display
+                    # Scale the right argument according to the legend width
+                    self.fig.subplots_adjust(right=1 - legend_width_scaled)
+                    # Place the legend outside the axis
+                    self.ax.legend(loc='center left',bbox_to_anchor=(1, 0.8))
+                    # Adjust figure size to increase width according to the outside legend width
+                    fig_size = plt.gcf().get_size_inches()
+                    fig_size[0] = fig_size[0] + fig_size[0]*(legend_width_scaled) # Increase width by the padding
+                    plt.gcf().set_size_inches(fig_size)
                 else:
                     self.ax.legend()
                 # Adjust layout to prevent overlapping of titles and labels
                 plt.tight_layout()
                 # Redraw the plot
                 plt.draw()
             def on_key_press(self, event):
@@ -498,100 +515,100 @@
                 fig_box = plt.gcf().get_window_extent()
                 fig_width_display = fig_box.width
                 # See by what fraction the figure width needs to be extended for outside legend.
                 legend_width_scaled=legend_width/fig_width_display
                 # Scale the right argument according to the legend width
                 plt.subplots_adjust(right=1 - legend_width_scaled)
                 # Place the legend outside the axis
-                plt.legend(loc='center left', bbox_to_anchor=(1, 0.78))
+                plt.legend(loc='center left', bbox_to_anchor=(1, 0.8))
                 # Adjust figure size to increase width according to the outside legend width
                 fig_size = plt.gcf().get_size_inches()
                 fig_size[0] = fig_size[0] + fig_size[0]*(legend_width_scaled) # Increase width by the padding
                 plt.gcf().set_size_inches(fig_size)
             else:
                 plt.legend()
             if ylim!=None:
                 plt.ylim(0,ylim)
             #Use plt.show to complete plot and move to the next reaction mixture data set
             plt.show()
 
-def plot_data_together(data,species,ylim=None,y_unit='mM',fig_size_scaler=1,t_unit=None,legend_outside=False,
-    DP_scaler=1,linewidth=1):
+def plot_data_together(data,species,ylim=None,y_unit='mM',fig_size_scaler=1,t_unit=None,
+    legend_outside=False,DP_scaler=1,linewidth=1):
     """
     Inputs the kinetic data "data" that has been imported from an excel file using Pd.read_excel() \
     as a dictionary of DataFrames containing the concentration profiles for each different excess \
     experiment. Creates a plot with the concentration profiles of the selected reaction species from \
     each experiment. 
     Args:
         data (dict): Kinetic data as a dictionary of Pandas dataframes.
         species (list): List containing the reaction species whose concentration profiles \
         will be plotted. 
         ylim (float or int, optional): Y axis upper cutoff value so that Y∈[0,ylim]. 
         y_unit (str, optional): Concentration unit to be included in the Y axis label.
         fig_size_scaler (float or int, optional): Scaler to adjust the size of the graphs by the \
         selected factor.
-        t_unit (str): Unit of the time axis. Set to None by default (assuming the time unit is already \
-        provided in the time column of the kinetic data). Can be set to any string like 'min' or 'h'.
-        legend_outside (bol): Set to True to ensure that the to place the plot legend to the right \
-        of the plot axis object. Set to False (by default) to show the legend in the main plot window.\
-        DP_scaler (float or int): Number by which the datapoints are scaled away from the standard size of 6. \
-        Can be set to 0 to remove datapoints all together.  
-        linewidth (float or int): Defines the linewidth of the graphs in the plot. Can be set to 0 to remove \
-        lines all together.  
+        t_unit (str): Unit of the time axis. Gives a "/ " followed by the string as an addition to \
+        the column title of the time column in the inputted kinetic dataset. 
+        legend_outside (bol): Set to False by default to show legend inside the axis of the plot. \
+        Can be set to True to show the legend outside the axis (top right). 
+        DP_scaler (float, int): Factor by which the datapoints of the plots is scaled from a standard \
+        value of 6. 
+        linewidth (float, int): The linewidth parameter used to generate plots. Is by default set to 1. 
     """
     # Identify the first key in the data dictionary
     RM1=list(data.keys())[0]
     # Identify the time column unit for the first reaction mixture data set
     t=data[RM1].columns[0]
     # Set the datapoint size scaler to 1 if an incorrect value has been assigned.
     if DP_scaler==None or isinstance(DP_scaler, str):
         DP_scaler=1
     t_label=t
     if t_unit!=None:
         t_label=t_label+f' / {t_unit}'
-    fig, ax = plt.subplots(figsize=(7*0.8*fig_size_scaler, 5*0.8*fig_size_scaler))
+    fig, ax = plt.subplots(figsize=(7*0.9*fig_size_scaler, 5*0.9*fig_size_scaler))
     for i in data.keys():
         time=data[i][t]
         # plot kinetic profiles for the chosen species for each reaction mixture data set
         for j in data[i].keys():
             if j==t or j not in species:
                 continue
-            ax.plot(time,data[i][j],label=f'{i}, {j}',linestyle='-',marker='o',markersize=6*DP_scaler,linewidth=linewidth)
+            ax.plot(time,data[i][j],label=f'{i},{species}',linestyle='-',marker='o',
+                    markersize=6*DP_scaler,linewidth=linewidth)
             ax.set_title(f'concentration profiles for {species}')
             ax.set_xlabel(t_label)
             ax.set_ylabel(f'concentration / {y_unit}')
         # Define y-axis range up to ylim if defined.
         if ylim!=None:
-            ax.ylim(0,ylim)
+            ax.set_ylim(0,ylim)
     if legend_outside:
         # Calculate the width of the legend dynamically based on the longest text element
         legend = plt.legend()
         # Obtain the legend width in display units. 
         legend_bbox = legend.get_window_extent()
         legend_width = legend_bbox.width
         # Obtain the figure width in display units.
         fig_box = plt.gcf().get_window_extent()
         fig_width_display = fig_box.width
         # See by what fraction the figure width needs to be extended for outside legend.
         legend_width_scaled=legend_width/fig_width_display
         # Scale the right argument according to the legend width
         plt.subplots_adjust(right=1 - legend_width_scaled)
         # Place the legend outside the axis
-        plt.legend(loc='center left', bbox_to_anchor=(1, 0.78))
+        plt.legend(loc='center left',bbox_to_anchor=(1, 0.8))
         # Adjust figure size to increase width according to the outside legend width
         fig_size = plt.gcf().get_size_inches()
         fig_size[0] = fig_size[0] + fig_size[0]*(legend_width_scaled) # Increase width by the padding
         plt.gcf().set_size_inches(fig_size)
     else:
         ax.legend()
     plt.tight_layout()
     plt.show()
 
-def plot_data_MB(data, species, stochiometry, scaler=1, ylim=None, t_unit=None, y_unit='mM', 
-    fig_size_scaler=1,plot_mode='together',legend_outside=False,DP_scaler=1,linewidth=1):
+def plot_data_MB(data, species, stochiometry, scaler=1, ylim=None, t_unit=None, y_unit='mM', fig_size_scaler=1,
+                 plot_mode='together',legend_outside=False,DP_scaler=1,linewidth=1):
     """
     Inputs the kinetic data "data" that has been imported from an excel file using Pd.read_excel() \
     as a dictionary of DataFrames containing the concentration profiles for each different excess \
     experiment. Plots the concentration profiles of each each experiment with the mass balance relative \
     to time=0 of the chosen reaction species and their stochiometries. The graphs can be plotted in one \
     figure (plot_mode = 'together'), in separate pop-up figures (plot_mode='separate') or in a single \
     figure that can be updated upon 
@@ -605,46 +622,37 @@
         y_unit (str, optional): Concentration unit to be included in the Y axis label.
         fig_size_scaler (float or int, optional): Scaler to adjust the size of the graphs by the \
         selected factor.
         plot_mode (str): Either set to "scrollable" to generate a single graph which updates \
         to the next or previous graph by clicking right or left arrow keys, or 'together' to \
         plot graphs for each experiment together. If plot_mode is set to something else, \
         graphs will pop-up one after the other. 
-        legend_outside (bol): Set to True to ensure that the to place the plot legend to the right \
-        of the plot axis object, or in a separate box if plot_mode=together. Set to False (by default) \
-        to show the legend in the main plot(s)
-        DP_scaler (float or int): Number by which the datapoints are scaled away from the standard size of 6. \
-        Can be set to 0 to remove datapoints all together.  
-        linewidth (float or int): Defines the linewidth of the graphs in the plot. Can be set to 0 to remove \
-        lines all together.  
+        legend_outside (bol): Set to False by default to show legend inside the axis of the plot. \
+        Can be set to True to show the legend outside the axis (top right). 
+        DP_scaler (float, int): Factor by which the datapoints of the plots is scaled from a standard \
+        value of 6. 
+        linewidth (float, int): The linewidth parameter used to generate plots. Is by default set to 1. 
     """
     # Find the title of the time column of the experiment datasets
     RM1 = list(data.keys())[0]
     t = data[RM1].columns[0]
     # Set the datapoint size scaler to 1 if an incorrect value has been assigned.
     if DP_scaler==None or isinstance(DP_scaler, str):
         DP_scaler=1
     MB_title_string = ''
-    # Set the datapoint size scaler to 1 if an incorrect value has been assigned.
-    if DP_scaler==None or isinstance(DP_scaler, str):
-        DP_scaler=1
     # Define the title of the mass balance axis
     for mol in range(len(species)):
         if mol != 0 and species[mol] == species[-1]:
             MB_title_string = MB_title_string + 'and '
         MB_title_string = MB_title_string + f'{species[mol]}, '
     if len(species) == 1:
         MB_title_string = f'{species[0]}. '
     if plot_mode == 'together':
-        addition=0
-        if legend_outside:
-            addition=1
-        # Check how many r
         # define the number of columns and rows for the subplot. 
-        n,m = len(list(data.keys()))+addition,3
+        n,m = len(list(data.keys()))+1,3
         if n>6:
             m=4
         num_cols = min(m, n)
         num_rows = (n + num_cols - 1) // num_cols  # Equivalent to ceil(n / num_cols)
         # Create subplots
         fig, axes = plt.subplots(num_rows, num_cols, figsize=(7 * 0.8*fig_size_scaler * num_cols, 5 *0.8* num_rows * fig_size_scaler))
         axes = axes.flatten() 
@@ -673,15 +681,16 @@
             sums = np.zeros(len(Concs[0]))
             for i in Concs:
                 sums = sums + i
             # Use sums to find the % mass balance at each time relative to the initial value.
             MB = sums / sums[0] * 100 * scaler
             ax2 = ax.twinx()
             ax2.set_ylabel(f'Mass balance for:\n {MB_title_string[:-2]}', color="purple")
-            ax2.plot(time, MB, label="Mass balance %", linestyle='-', marker='o', color="purple",markersize=6*DP_scaler,linewidth=linewidth)
+            ax2.plot(time, MB, label="Mass balance %", linestyle='-', marker='o', color="purple",
+                     markersize=6*DP_scaler,linewidth=linewidth)
             ax2.plot([0, max(time)], [100, 100], linestyle='--', marker='', color='purple')
             ax2.legend(loc='upper center')
             # Ensure appropriate y limits with space for legends.
             ax2.set_ylim(0, max(MB) + 28)
             ax.set_ylim(0, max(largest_conc) + max(largest_conc) * 0.15)
         ax = axes[idx+1]
         handles, labels = axes[0].get_legend_handles_labels()
@@ -690,15 +699,15 @@
         ax.spines['left'].set_visible(False)
         ax.spines['bottom'].set_visible(False)
         ax.set_xticklabels([])
         ax.set_yticklabels([])
         ax.set_xticks([])
         ax.set_yticks([])
         ax.legend(handles, labels, loc='center left')
-        for i in range(len(data)+addition, num_cols * num_rows):
+        for i in range(len(data)+1, num_cols * num_rows):
           fig.delaxes(axes.flatten()[i])
         # Adjust layout to prevent overlap
         plt.subplots_adjust(wspace=1.45, hspace=1.45)
         plt.tight_layout()
         plt.show()
     elif plot_mode=='scrollable':
         class ScrollablePlot:
@@ -720,15 +729,15 @@
                 self.legend_outside=legend_outside
                 self.DP_scaler=DP_scaler
                 self.linewidth=linewidth
                 mplcursors.cursor(hover=True)
                 self.fig, self.ax = plt.subplots(figsize=(7 *0.8* fig_size_scaler, 5 *0.8* fig_size_scaler))
                 # Create a note to inform user of scrolling feature.
                 note_text = 'NB: Use left or right arrows to scroll to other experiments.'
-                self.fig.text(0.5, 0.003, note_text, ha='center', color='gray')
+                self.fig.text(0.5, 0.015, note_text, ha='center', color='gray')
                 self.ax2=self.ax.twinx()
                 self.plot_current_data()
                 self.fig.canvas.mpl_connect('key_press_event', self.on_key_press)
 
             def plot_current_data(self):
                 self.ax.clear()
                 self.ax2.clear()
@@ -737,15 +746,16 @@
                 t=current_data.columns[0]
                 time_column=current_data[t]
                 Concs=[]
                 largest_conc=[]
                 for j in current_data.keys():
                     if j==t:
                         continue
-                    self.ax.plot(time_column,current_data[j],label=j,linestyle='-',marker='o',markersize=6*self.DP_scaler,linewidth=self.linewidth)
+                    self.ax.plot(time_column,current_data[j],label=j,linestyle='-',marker='o',
+                                 markersize=6*self.DP_scaler,linewidth=linewidth)
                     self.ax.set_title(f'Concentration profiles in {current_label}')
                     self.fig.set_size_inches(7*0.8*self.fig_size_scaler, 5*0.8*self.fig_size_scaler)
                     self.ax.set_xlabel(t)
                     self.ax.set_ylabel(f'concentration / {self.y_unit}')
                     if self.ylim!=None:
                         self.ax.set_ylim(0,self.ylim)
                     largest_conc.append(max(current_data[j].to_numpy()))
@@ -759,15 +769,16 @@
                 sums=np.zeros(len(Concs[0]))
                 for i in Concs:
                     sums=sums+i
                 # Use sums to find the % mass balance at each time relative to the intial value.
                 MB=sums/sums[0]*100* scaler
                 self.ax2.set_ylabel(f'Mass balance for:\n {self.MB_title_string[:-2]}',color="purple")
                 self.ax2.yaxis.set_label_position('right')
-                self.ax2.plot(time_column,MB,label="Mass balance %",linestyle='-',marker='o',color="purple",markersize=6*self.DP_scaler,linewidth=self.linewidth)
+                self.ax2.plot(time_column,MB,label="Mass balance %",linestyle='-',marker='o',color="purple",
+                              markersize=6*self.DP_scaler,linewidth=linewidth)
                 self.ax2.plot([0,max(time_column)],[100,100],linestyle='--',marker='',color='purple')
                 self.ax2.legend(loc='upper center')
                 # Ensure appropriate y limits with space for legends. 
                 self.ax2.set_ylim(0,max(MB)+28)
                 self.ax.set_ylim(0,max(largest_conc)+max(largest_conc)*0.15)
                 if self.legend_outside:
                     # Calculate the width of the legend dynamically based on the longest text element
@@ -777,17 +788,17 @@
                     legend_width = legend_bbox.width
                     # Obtain the figure width in display units.
                     fig_box = plt.gcf().get_window_extent()
                     fig_width_display = fig_box.width
                     # See by what fraction the figure width needs to be extended for outside legend.
                     legend_width_scaled=legend_width/fig_width_display
                     # Scale the right argument according to the legend width
-                    self.fig.subplots_adjust(right=1 - legend_width_scaled)
+                    self.fig.subplots_adjust(right=1 - legend_width_scaled-0.06)
                     # Place the legend outside the axis
-                    self.ax.legend(loc='center left', bbox_to_anchor=(1.17, 0.8))
+                    self.ax.legend(loc='center left',bbox_to_anchor=(1.16, 0.8))
                     # Adjust figure size to increase width according to the outside legend width
                     fig_size = plt.gcf().get_size_inches()
                     fig_size[0] = fig_size[0] + fig_size[0]*(legend_width_scaled) # Increase width by the padding
                     plt.gcf().set_size_inches(fig_size)
                 else:
                     self.ax.legend()
                 plt.tight_layout()
@@ -810,45 +821,66 @@
         plt.show()
     else: 
         # Create a twin plot for each experiment dataset
         for i in data.keys():
             Concs=[]
             largest_conc=[]
             fig,ax = plt.subplots(figsize=(7*0.8*fig_size_scaler, 5*0.8*fig_size_scaler))
+            fig_size = plt.gcf().get_size_inches()
             time=data[i][t]
             # Create a curve for each reaction species
             for j in data[i].keys():
                 if j==t:
                     continue
-                ax.plot(time,data[i][j],label=j,linestyle='-',marker='o',markersize=6*DP_scaler,linewidth=linewidth)
+                ax.plot(time,data[i][j],label=j,linestyle='-',marker='o',
+                        markersize=6*DP_scaler,linewidth=linewidth)
                 ax.set_title(i)
                 ax.set_xlabel(t)
                 ax.set_ylabel(f'concentration / {y_unit}')
-                if ylim!=None:
-                    ax.set_ylim(0,ylim)
-                if legend_outside:
-                    ax.legend(bbox_to_anchor=(1,0.78))
-                else:
-                    ax.legend()
                 largest_conc.append(max(data[i][j].to_numpy()))
                 if t_unit!=None:
                     plt.xlabel(f'{t} / {t_unit}')
                 if j==t or j not in species:
                     continue
                 # Add concentration*stochiometry array for calculation of mass balance over time
                 Concs.append(data[i][j].to_numpy()*stochiometry[species.index(j)])
+            if ylim!=None:
+                ax.set_ylim(0,ylim)
+            if legend_outside:
+                # Calculate the width of the legend dynamically based on the longest text element
+                legend = ax.legend()
+                # Obtain the legend width in display units. 
+                legend_bbox = legend.get_window_extent()
+                legend_width = legend_bbox.width
+                # Obtain the figure width in display units.
+                fig_box = plt.gcf().get_window_extent()
+                fig_width_display = fig_box.width
+                # See by what fraction the figure width needs to be extended for outside legend.
+                legend_width_scaled=legend_width/fig_width_display
+                # Scale the right argument according to the legend width
+                fig.subplots_adjust(right=1 - legend_width_scaled-0.06)
+                # Place the legend outside the axis
+                ax.legend(loc='center left', bbox_to_anchor=(1.16, 0.8))
+                # Adjust figure size to increase width according to the outside legend width
+                fig_size = plt.gcf().get_size_inches()
+                fig_size[0] = fig_size[0] + fig_size[0]*(legend_width_scaled) # Increase width by the padding
+                plt.gcf().set_size_inches(fig_size)
+            else:
+                ax.legend()
             # Use Concs to create mass balance sum for each time point
             sums=np.zeros(len(Concs[0]))
             for i in Concs:
                 sums=sums+i
             # Use sums to find the % mass balance at each time relative to the intial value.
             MB=sums/sums[0]*100*scaler
             ax2=ax.twinx()
             ax2.set_ylabel(f'Mass balance for:\n {MB_title_string[:-2]}',color="purple")
-            ax2.plot(time,MB,label="Mass balance %",linestyle='-',marker='o',color="purple",markersize=6*DP_scaler,linewidth=linewidth)
-            ax2.plot([0,max(time)],[100,100],linestyle='--',marker='',color='purple',markersize=6*DP_scaler,linewidth=linewidth)
+            ax2.plot(time,MB,label="Mass balance %",linestyle='-',marker='o',color="purple",
+                     markersize=6*DP_scaler,linewidth=linewidth)
+            ax2.plot([0,max(time)],[100,100],linestyle='--',marker='',color='purple',
+                     markersize=6*DP_scaler,linewidth=linewidth)
             ax2.legend(loc='upper center')
             # Ensure appropriate y limits with space for legends. 
             ax2.set_ylim(0,max(MB)+28)
             ax.set_ylim(0,max(largest_conc)+max(largest_conc)*0.15)
             plt.show()
```

### Comparing `auto_vtna-1.0.1/auto_vtna/running_codes 23dec.py` & `auto_vtna-1.0.2/auto_vtna/running_codes 23dec.py`

 * *Files 21% similar despite different names*

```diff
@@ -21,22 +21,25 @@
 # del data_VTNA2['RM1']
 #vtna=Normal_VTNA(data_VTNA2,selection_VTNA2_a)
 #vtna.plot_VTNA_with_overlay_score(DP_scaler=1,xtick_rotation=20,constraint='j',deg=1,fit_metric='RMSE',show_legend=True,legend_outside=True,size_scaler=1.2)
 #vtna.plot_VTNA_with_overlay_score(constraint='origin',show_legend=True,legend_outside=True)
 #vtna.plot_VTNA(legend_outside=True,show_legend=False)
 #vtna.plot_VTNA_with_overlay_score(size_scaler=0.9,constraint=None,deg=2,fit_metric='through_origin',show_fit_function=True,show_overlay_score=False)
 #plt.show()
-plot_data_MB(data_VTNA2,['RBr','Styrene', 'Prod'],[1,1,1],legend_outside=True,plot_mode='scrollable')
-#plot_data(data_VTNA2,plot_mode='together',legend_outside=False)
-#plot_data(bull_data,plot_mode='together',legend_outside=True)
-#plot_data_MB(data_VTNA2,['RBr','Prod'],[1,1],plot_mode='together',fig_size_scaler=1,legend_outside=True)
+plot_data_MB(data_VTNA2,['RBr','Styrene', 'Prod'],[1,1,1],legend_outside=True,plot_mode='scrollable',linewidth=0,DP_scaler=2)
+plot_data(data_VTNA2,plot_mode='together',legend_outside=False)
+plot_data(bull_data,plot_mode='together',legend_outside=True)
+#plot_data_MB(data_VTNA2,['RBr','Prod'],[1,1],plot_mode='scrollable',fig_size_scaler=1,legend_outside=True)
+#plot_data_MB(data_VTNA2,['RBr','Prod'],[1,1],plot_mode='sc',fig_size_scaler=1,legend_outside=True)
 #plot_data_MB(data_THF,['A','P'],[1,1],plot_mode='together',fig_size_scaler=1,legend_outside=False)
-#plot_data(data_VTNA2,plot_mode='together')
+#plot_data(data_VTNA2,plot_mode='separate',legend_outside=True)
+plot_data(data_VTNA2,plot_mode='scrollable',legend_outside=True,linewidth=0,DP_scaler=2)
+#plot_data(data_VTNA2,plot_mode='scrf',legend_outside=True)
 #plot_data(data_THF,plot_mode='together')
-plot_data_together(data_VTNA2,['RBr'],legend_outside=True)
+#plot_data_together(data_VTNA2,['RBr'],legend_outside=True)
 #plot_data_2(data_VTNA2,plot_mode='scrollable',fig_size=1)
 #vtna2_a=Automatic_VTNA(data_VTNA2,selection_VTNA2_a,constraint=None,fixed_order_species='RBr')
 #vtna2_a=Automatic_VTNA(data_VTNA2,selection_VTNA2_a,constraint='monotonic')
 #vtna2_b=Automatic_VTNA(data_VTNA2,selection_VTNA2_a,constraint=None,fixed_order_species='RBr',deg=7)
 #vtna2_c=Automatic_VTNA(data_VTNA2,selection_VTNA2_a,fixed_order_species='RBr',deg=1,constraint='origin')
 #vtna2_a.plot_orders_vs_overlay(interval=True,points=True)
 #vtna2_b.plot_orders_vs_overlay(interval=True)
```

### Comparing `auto_vtna-1.0.1/auto_vtna.egg-info/PKG-INFO` & `auto_vtna-1.0.2/auto_vtna.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-vtna
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python package for efficient and automatic VTNA analysis
 Author: Daniel Dalland
 Author-email: dd4518@ic.ac.uk
 License: MIT
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
```

### Comparing `auto_vtna-1.0.1/setup.py` & `auto_vtna-1.0.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,23 +2,25 @@
 from os import path
 
 # Meta-data of the package.
 NAME = 'auto_vtna'
 DESCRIPTION = 'A Python package for efficient and automatic VTNA analysis'
 EMAIL = 'dd4518@ic.ac.uk'
 AUTHOR = 'Daniel Dalland'
-VERSION = "1.0.1"
-REQUIRED = [
-    'numpy',
+VERSION = "1.0.2"
+REQUIRED=[
     'pandas',
+    'numpy',
     'matplotlib',
-    'polyfit',
     'num2words',
-    'scikit-learn',
-    'scipy'
+    'mplcursors',
+    'scipy',
+    'polyfit',
+    'PySimpleGUI',
+    'openpyxl',
 ]
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
```

