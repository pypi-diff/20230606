# Comparing `tmp/pyseafuel-0.1.1.tar.gz` & `tmp/pyseafuel-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyseafuel-0.1.1.tar", max compression
+gzip compressed data, was "pyseafuel-0.1.2.tar", max compression
```

## Comparing `pyseafuel-0.1.1.tar` & `pyseafuel-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35149 2022-02-24 11:57:16.952331 pyseafuel-0.1.1/LICENSE
--rw-r--r--   0        0        0      439 2022-08-11 07:08:38.508226 pyseafuel-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      208 2022-06-09 13:46:48.711949 pyseafuel-0.1.1/pyseafuel/__init__.py
--rw-r--r--   0        0        0      678 2022-06-10 15:33:28.732224 pyseafuel-0.1.1/pyseafuel/_constants.py
--rw-r--r--   0        0        0     2600 2022-06-09 13:05:47.226028 pyseafuel-0.1.1/pyseafuel/degasser.py
--rw-r--r--   0        0        0     8169 2022-06-13 16:29:27.091791 pyseafuel-0.1.1/pyseafuel/desalinator.py
--rw-r--r--   0        0        0     6401 2022-06-19 18:26:56.850344 pyseafuel-0.1.1/pyseafuel/dic.py
--rw-r--r--   0        0        0     4611 2022-06-12 17:56:52.519664 pyseafuel-0.1.1/pyseafuel/electrolyzer.py
--rw-r--r--   0        0        0    10008 2022-06-13 22:08:50.613735 pyseafuel-0.1.1/pyseafuel/reactor.py
--rw-r--r--   0        0        0     5879 2022-08-02 01:19:40.518928 pyseafuel-0.1.1/pyseafuel/system.py
--rw-r--r--   0        0        0      692 2022-08-12 07:08:33.213973 pyseafuel-0.1.1/setup.py
--rw-r--r--   0        0        0      418 2022-08-12 07:08:33.214132 pyseafuel-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-02-24 11:57:16.952331 pyseafuel-0.1.2/LICENSE
+-rw-r--r--   0        0        0      433 2023-06-06 12:54:45.959366 pyseafuel-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      772 2022-09-16 15:20:47.651968 pyseafuel-0.1.2/pyseafuel/__init__.py
+-rw-r--r--   0        0        0      678 2022-06-10 15:33:28.732224 pyseafuel-0.1.2/pyseafuel/_constants.py
+-rw-r--r--   0        0        0     2669 2022-09-16 14:42:19.602320 pyseafuel-0.1.2/pyseafuel/degasser.py
+-rw-r--r--   0        0        0     8325 2022-09-16 14:47:21.113580 pyseafuel-0.1.2/pyseafuel/desalinator.py
+-rw-r--r--   0        0        0     6512 2022-09-16 15:04:07.840943 pyseafuel-0.1.2/pyseafuel/dic.py
+-rw-r--r--   0        0        0     4644 2022-09-16 15:06:02.759368 pyseafuel-0.1.2/pyseafuel/electrolyzer.py
+-rw-r--r--   0        0        0    10116 2022-09-16 15:10:27.702154 pyseafuel-0.1.2/pyseafuel/reactor.py
+-rw-r--r--   0        0        0     5494 2022-09-16 15:18:46.963890 pyseafuel-0.1.2/pyseafuel/system.py
+-rw-r--r--   0        0        0      686 2023-06-06 12:54:53.546879 pyseafuel-0.1.2/setup.py
+-rw-r--r--   0        0        0      463 2023-06-06 12:54:53.547029 pyseafuel-0.1.2/PKG-INFO
```

### Comparing `pyseafuel-0.1.1/LICENSE` & `pyseafuel-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyseafuel-0.1.1/pyseafuel/_constants.py` & `pyseafuel-0.1.2/pyseafuel/_constants.py`

 * *Files identical despite different names*

### Comparing `pyseafuel-0.1.1/pyseafuel/degasser.py` & `pyseafuel-0.1.2/pyseafuel/degasser.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,19 +18,19 @@
     mass_co2_out : float
         Mass flow rate out of degassed carbon dioxide; kilogram per second.
     power_consumed : float
         Power consumed to operate the electrodialysis device; Watts.
 
     Notes
     -----
-    This function estimates the carbon dioxide extraction flow rate and power consumption from sea water from the data found in Table SI in [1]_. [1]_ outlines and tests a prototype bipolar membrane electrodialysis device that separates the inflow sea water into a basified and acidified stream, extracting carbon dioxide from the acified stream.
+    This function estimates the carbon dioxide extraction flow rate and power consumption from sea water from the data found in Table SI in Eisaman et al. 2012[1]_. Eisaman et al. 2012 outlines and tests a prototype bipolar membrane electrodialysis device that separates the inflow sea water into a basified and acidified stream, extracting carbon dioxide from the acified stream.
 
     References
     ----------
-    .. [1] M. Eisaman, K. Parajuly, A. Tuganov, C. Eldershaw, N. Chang, and K. Littau, "CO:sub:`2` extraction from seawater using bipolar membrane electrodialysis," vol. 5, pp. 7346-7352, 2012.
+    .. [1] `M. Eisaman, K. Parajuly, A. Tuganov, C. Eldershaw, N. Chang, and K. Littau, "CO$_2$ extraction from seawater using bipolar membrane electrodialysis," vol. 5, pp. 7346-7352, 2012.<https://doi.org/10.1039/C2EE03393C>`_
     """
 
     def flow_ratio_from_pH(pH):
         """
         Ratio of carbon dioxide out to seawater in. Fitted from data from Table SI from [1]_.
         """
```

### Comparing `pyseafuel-0.1.1/pyseafuel/desalinator.py` & `pyseafuel-0.1.2/pyseafuel/desalinator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pyseafuel._constants as _constants
 import numpy as np
 
 # ──────────────────────────────────────────────────────────────────────────
 
 def ideal(volume_seawater_in, S, T, water_ratio, efficiency=1, brine_concentration=False):
     """
-    Thermodynamic limit for desalinating an inflow of saline water to produce pure water.
+    Thermodynamic limit for desalinating an inflow of saline water to produce pure water[1]_.
 
     Parameters
     ----------
     volume_seawater_in : float
         Seawater inflow; liters per second.
     S : float
         Seawater inflow salinity; Practical Salinity Units.
@@ -33,15 +33,15 @@
     power_consumed : float
         Power consumed by the desalination process, in Watts.
     c_b : float (optional)
         Brine molar concentration, in moles per liter.
 
     References
     ----------
-    .. [1] L. Wang, C. Violet, R. DuChanois, and M. Elimelech, "Derivation of the Theoretical Minimum Energy of Separation of Desalination Process," Journal of Chemical Education, vol. 97, pp. 4361-4369, 2020.
+    .. [1] `L. Wang, C. Violet, R. DuChanois, and M. Elimelech, "Derivation of the Theoretical Minimum Energy of Separation of Desalination Process," Journal of Chemical Education, vol. 97, pp. 4361-4369, 2020.<https://doi.org/10.1021/acs.jchemed.0c01194>`_
     """
 
     # molar concentration of salt in inflow
     ppt = S  # PSU approxiamtely equal to parts per thousand (PPT); which is essentially in g/L;
     c_f = ppt / _constants.mol_weight_nacl / 1000  # mol/L
 
     pi_f = 2 * _constants.R * T * c_f   # J/L; osmotic pressure of sea water
@@ -60,15 +60,15 @@
         return volume_h2o_out, volume_brine_out, power_consumed, c_b
 
     return volume_h2o_out, volume_brine_out, power_consumed
 
 
 def reverse_osmosis(volume_seawater_in, S, T, water_ratio, stages, brine_concentration=False):
     """
-    Multistage reverse osmosis desalinator for desalinating an inflow of saline water to produce pure water.
+    Multistage reverse osmosis desalinator for desalinating an inflow of saline water to produce pure water[1]_.
 
     Parameters
     ----------
     volume_seawater_in : float
         Seawater inflow; liters per second.
     S : float
         Seawater inflow salinity; Practical Salinity Units.
@@ -90,15 +90,15 @@
     power_consumed : float
         Power consumed by the desalination process; Watts.
     c_b : float (optional)
         Brine molar concentration; moles per liter.
 
     References
     ----------
-    .. [1] L. Wang, C. Violet, R. DuChanois, and M. Elimelech, "Derivation of the Theoretical Minimum Energy of Separation of Desalination Process," Journal of Chemical Education, vol. 97, pp. 4361-4369, 2020.
+    .. [1] `L. Wang, C. Violet, R. DuChanois, and M. Elimelech, "Derivation of the Theoretical Minimum Energy of Separation of Desalination Process," Journal of Chemical Education, vol. 97, pp. 4361-4369, 2020.<https://doi.org/10.1021/acs.jchemed.0c01194>`_
     """
 
     def _water_ratio_i(water_ratio, stages, i):
         """Water ratio per stage.
         """
 
         water_ratio_i = water_ratio * i / ((1 - water_ratio) * stages + water_ratio * i)
@@ -132,15 +132,15 @@
         return volume_h2o_out, volume_brine_out, power_consumed, c_b
 
     return volume_h2o_out, volume_brine_out, power_consumed
 
 
 def electrodialysis(volume_seawater_in, S, T, water_ratio, salt_removal, stages, brine_concentration=False):
     """
-    Multistage electrodialysis desalinator for desalinating an inflow of saline water to produce pure water.
+    Multistage electrodialysis desalinator for desalinating an inflow of saline water to produce pure water[1]_.
 
     Parameters
     ----------
     volume_seawater_in : float
         Seawater inflow; liters per second.
     S : float
         Seawater inflow salinity; Practical Salinity Units.
@@ -164,15 +164,15 @@
     power_consumed : float
         Power consumed by the desalination process; Watts.
     c_b : float (optional)
         Brine molar concentration; moles per liter.
 
     References
     ----------
-    .. [1] L. Wang, C. Violet, R. DuChanois, and M. Elimelech, "Derivation of the Theoretical Minimum Energy of Separation of Desalination Process," Journal of Chemical Education, vol. 97, pp. 4361-4369, 2020.
+    .. [1] `L. Wang, C. Violet, R. DuChanois, and M. Elimelech, "Derivation of the Theoretical Minimum Energy of Separation of Desalination Process," Journal of Chemical Education, vol. 97, pp. 4361-4369, 2020.<https://doi.org/10.1021/acs.jchemed.0c01194>`_
     """
     
     # per stage values
     salt_removal_i = 1 - (1 - salt_removal)**(1/stages)  # salt removal percentage per stage in terms of concentration
     water_ratio_i = water_ratio**(1/stages)  # water ratio per stage
 
     # Calculating inflow salt molar concentration
```

### Comparing `pyseafuel-0.1.1/pyseafuel/dic.py` & `pyseafuel-0.1.2/pyseafuel/dic.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,31 +19,35 @@
         Pressure at the air-sea interface; Pa; default = 101325 Pa.
     volume : bool (optional)
         Whether or not to calculate dissolved carbon dioxide in mol/L or mol/kg.
 
     Returns
     -------
     co2 : float
-        Dissolved carbon dioxide and carbonic acid in the ocean; mol/L or mol/kg (see 'volume'); defaults to mol/L.
+        Dissolved carbon dioxide and carbonic acid in the ocean; mol/L or mol/kg (see **volume**); defaults to mol/L.
 
     Notes
     -----
-    [CO:sub:`2`] includes dissolved CO:sub:`2` and H:sub:`2`CO:sub:`3`, as they are hard to distinguish in experiments.
+    [CO$_2$] includes dissolved CO$_2$ and H$_2$CO$_3$, as they are hard to distinguish in experiments.
 
-    From [1]_:
+    From Weiss 1974[1]_:
 
-    .. math:: [CO_2] = K f_{CO_2} e^{(1 - P) v_{CO_2} / RT}
+    $$
+    [CO_2] = K f_{CO_2} e^{(1 - P) v_{CO_2} / RT}
+    $$
 
     However, when pressure is close to 1 atm, we can assume the exponential term goes to 1:
     
-    .. math:: [CO_2] = K * f_{CO_2} 
+    $$
+    [CO_2] = K * f_{CO_2} 
+    $$
 
     References
     ----------
-    .. [1] R. F. Weiss "Carbon Dioxide in Water and Seawater: The Solubility of a Non-ideal Gas," Marine Chemistry, vol. 2, pp. 203-216, 1974.
+    .. [1] `R. F. Weiss "Carbon Dioxide in Water and Seawater: The Solubility of a Non-ideal Gas," Marine Chemistry, vol. 2, pp. 203-216, 1974.<https://doi.org/10.1016/0304-4203(74)90015-2>`_
     """
 
     if volume:
         # constants for volume basis
         A = [-58.0931, 90.5069, 22.2940]
         B = [0.027766, -0.025888, 0.0050578]
 
@@ -86,38 +90,41 @@
     Returns
     -------
     hco3 : float
         Molar concentration of bicarbonate; moles per kilogram of solution.
 
     Notes
     -----
-    The coefficients come from [1]_.
+    The coefficients come from Lueker et al. 2000[1]_.
 
-    The dissolved CO:sub:`2` and H:sub:`2`CO:sub:`3` are hard to distinguish from one another in solution and are typically combined when calculating reaction equilibrium constants of the ocean buffer system [1]_.
+    The dissolved CO$_2$ and H$_2$CO$_3$ are hard to distinguish from one another in solution and are typically combined when calculating reaction equilibrium constants of the ocean buffer system.
 
-    pH is defined as:
+    $pH$ is defined as:
 
-    .. math:: pH = - \log(a_{H^+})
+    $$
+    pH = - \log(a_{H^+})
+    $$
 
-    However, here, it is assumed that :math:`a_{H^+} \approx [H^+]`.
+    However, here, it is assumed that $a_{H^+} \\approx [H^+]$.
 
     References
     ----------
-    .. [1] T. Lueker, A. Dickson, and C. Keeling, "Ocean pCO:sub:`2` calculated from dissolved inorganic carbon, alkalinity, and equations for K:sub:`1` and K:sub:`2`: validation based on laboratory measurements of CO:sub:`2` in gas and seawater at equilibrium," Marine Chemistry, vol. 70, pp. 105-119, 2000.
+    .. [1] `T. Lueker, A. Dickson, and C. Keeling, "Ocean pCO$_2$ calculated from dissolved inorganic carbon, alkalinity, and equations for K$_1$ and K$_2$: validation based on laboratory measurements of CO$_2$ in gas and seawater at equilibrium," Marine Chemistry, vol. 70, pp. 105-119, 2000.<https://doi.org/10.1016/S0304-4203(00)00022-0>`_
     """
 
     # pK1 = 3633.86/T - 61.2172 + 9.67770 * np.log(T) - 0.011555*S + 0.0001152*S**2
     # K1 = 10**(-pK1)
 
     K1 = 10**(-3633.86/T + 61.2172 - 9.67770*np.log(T) + 0.011555*S - 0.0001152*S**2)
 
     hco3 = K1 * co2 / 10**(-pH)
 
     return hco3
 
+
 def carbonate(T, S, hco3, pH):
     """
     Calculates the carbonate molar concentration of the ocean carbon buffer system at equilibrium.
 
     Parameters
     ----------
     T : float
@@ -132,25 +139,27 @@
     Returns
     -------
     co3 : float
         Molar concentration of bicarbonate; moles per kilogram of solution.
 
     Notes
     -----
-    The coefficients come from [1]_.
+    The coefficients come from Lueker et al. 2000[1]_.
 
-    pH is defined as:
+    $pH$ is defined as:
 
-    .. math:: pH = - \log_{10}(a_{H^+})
+    $$
+    pH = - \log_{10}(a_{H^+})
+    $$
 
-    However, here, it is assumed that :math:`a_{H^+} \approx [H^+]`.
+    However, here, it is assumed that :math:`a_{H^+} \\approx [H^+]`.
 
     References
     ----------
-    .. [1] T. Lueker, A. Dickson, and C. Keeling, "Ocean pCO:sub:`2` calculated from dissolved inorganic carbon, alkalinity, and equations for K:sub:`1` and K:sub:`2`: validation based on laboratory measurements of CO:sub:`2` in gas and seawater at equilibrium," Marine Chemistry, vol. 70, pp. 105-119, 2000.
+    .. [1] `T. Lueker, A. Dickson, and C. Keeling, "Ocean pCO$_2$ calculated from dissolved inorganic carbon, alkalinity, and equations for K$_1$ and K$_2$: validation based on laboratory measurements of CO$_2$ in gas and seawater at equilibrium," Marine Chemistry, vol. 70, pp. 105-119, 2000.<https://doi.org/10.1016/S0304-4203(00)00022-0>`_
     """
 
     # pK2 = 471.78/T + 25.9290 - 3.16967 * np.log(T) - 0.01781 * S + 0.0001122 * S**2
     # K2 = 10**(-pK2)
 
     K2 = 10**(-471.78/T - 25.9290 + 3.16967*np.log(T) + 0.01781*S - 0.0001122*S**2)
 
@@ -175,13 +184,15 @@
     Returns
     -------
     dic : float
         Molar concentration of dissolved inorganic carbon; moles per kilogram of solution.
 
     Notes
     -----
-    CO:sub:`2`:sup:`*` is the sum of CO:sub:`2` and H:sub:`2`CO:sub:`3`.
-    HCO:sub:`3`:sup:`-` is bicarbonate.
-    CO:sub:`3`:sup:`2-` is carbonate.
+    CO$_2^*$ is the sum of CO$_2$ and H$_2$CO$_3$.
+
+    HCO$_3^-$ is bicarbonate.
+
+    CO$_3^{2-}$ is carbonate.
     """
 
     return np.sum(co2, hco3, co3)
```

### Comparing `pyseafuel-0.1.1/pyseafuel/electrolyzer.py` & `pyseafuel-0.1.2/pyseafuel/electrolyzer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pyseafuel._constants as _constants
 import numpy as np
 
 # ──────────────────────────────────────────────────────────────────────────
 
-def mcphy_piel(volume_h2o_in):
+def Mcphy_Piel(volume_h2o_in):
     """
     Estimating power consumption and outflows for electrolyzing pure water with an McPhy Piel series electrolyzer.
 
     Parameters
     ----------
     volume_h2o_in : float
         Pure water inflow; liters per second.
@@ -19,17 +19,17 @@
     mass_o2_out : float
         Mass flow rate out of oxygen gas; kilograms per second.
     power_consumed : float
         Power consumed during electrolysis; Watts.
 
     Notes
     -----
-    The values to calculate the process of electrolysis come from the datasheet for the `McPhy Piel series H model electrolyzer. <https://mcphy.com/en/equipment-services/electrolyzers/small/>`_ It consumes 18 kW at an outflow of 3 m:sup:`3`/h of hydrogen and 60 kW at 10 m:sup:`3`/h.
+    The values to calculate the process of electrolysis come from the datasheet for the `McPhy Piel series H model electrolyzer. <https://mcphy.com/en/equipment-services/electrolyzers/small/>`_ It consumes 18 kW at an outflow of 3 m$^3$/h of hydrogen and 60 kW at 10 m$^3$/h.
 
-    This function is only accurate if the water inflow `volume_h2o_in` remains between 6.69 x 10:sup:`-4` L/s and 2.23 x 10:sup:`-3` L/s.
+    This function is only accurate if the water inflow **volume_h2o_in** remains between 6.69 x 10$^{-4}$ L/s and 2.23 x 10$^{-3}$ L/s.
     """
 
     volume_h2o_in /= 1000  # m^3/s; converting from liters to cubic meters
 
     ratio_h2_o2 = 2*_constants.rho_h2/_constants.rho_o2  # ratio of hydrogen over oxygen mass outflow rates
 
     # output volumes
@@ -59,38 +59,40 @@
     K : float
         Power conversion coefficient; unity per ohm squared centimeter.
     R : float
         Cell (internal) resistance; ohm squared centimeter.
     A : float
         Membrane stack area; squared centimeter.
     output_voltage : boolean
-        Flag to return voltage (V) with other return variables.
+        Flag to return voltage, **V**, with other return variables.
 
     Returns
     -------
     mass_h2_out : float
         Mass outflow of hydrogen; kilograms per second.
     mass_o2_out : float
         Mass outflow of oxygen; kilograms per second.
     power_consumed : float
         Power consumed during electrolysis.
     V : float (optional)
-        Operating voltage; V; see `output_voltage`.
+        Operating voltage, $V$; see **output_voltage**.
 
     Notes
     -----
-    Power calculation comes from the model in [1]_. Essentially, power is assumed to be proportional to the square of the cell voltage, ::math:`V`, internal resistance, ::math:`R`, and cell dissociatio potential, ::math:`E_0`:
+    Power calculation comes from the model in Shen et al. 2011[1]_. Essentially, power is assumed to be proportional to the square of the cell voltage, $V$, internal resistance, $R$, and cell dissociation potential, $E_0$:
 
-    .. math:: P = K ( V - IR - E_0)^2
+    $$
+    P = K ( V - IR - E_0)^2
+    $$
 
-    ::math:`K` and ::math:`R` are given in units with cm:sup:`2` because electrolysis processes are typically measured with current density rather than current.
+    $K$ and $R$ are given in units with cm$^2$ because electrolysis processes are typically measured with current density rather than current.
     
     References
     ----------
-    .. [1] N. Shen, N. Bennett, Y. Ding, and K. Scott, "A concise model for evaluating water electrolysis," International Journal of Hydrogen Energy, vol. 36, pp. 14335-14341, 2011.
+    .. [1] `N. Shen, N. Bennett, Y. Ding, and K. Scott, "A concise model for evaluating water electrolysis," International Journal of Hydrogen Energy, vol. 36, pp. 14335-14341, 2011.<http://dx.doi.org/10.1016/j.ijhydene.2010.12.029>`_
     """
 
     volume_h2o_in /= 1000  # m^3/s; converting from liters to cubic meters
     mass_h2o_in = volume_h2o_in * _constants.rho_h2o  # kg/s
 
     # molecular flow rates
     mol_h2o = mass_h2o_in / _constants.mol_weight_h2o
```

### Comparing `pyseafuel-0.1.1/pyseafuel/reactor.py` & `pyseafuel-0.1.2/pyseafuel/reactor.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,19 +34,19 @@
     N_h2o : float
         Equilibrium amount of water; moles.
     xi_3 : float
         Conversion factor of initial carbon dioxide to methanol.
 
     Notes
     -----
-    This numerical solution for the amounts of reactants/products at equilibrium for the hydrogenation of carbon monoxide follows the method laid out in [1]_.
+    This numerical solution for the amounts of reactants/products at equilibrium for the hydrogenation of carbon monoxide follows the method laid out in Terreni et al. 2020[1]_.
 
     References
     ----------
-    .. [1] J. Terreni, A. Borgschulte, M. Hillestad, and B. Patterson, "Understanding Catalysis-A Simplified Simulation of Catalytic Reactors for CO:sub:`2` Reduction," ChemEngineering, vol. 4, 2020.
+    .. [1] `J. Terreni, A. Borgschulte, M. Hillestad, and B. Patterson, "Understanding Catalysis-A Simplified Simulation of Catalytic Reactors for CO$_2$ Reduction," ChemEngineering, vol. 4, 2020.<https://doi.org/10.3390/chemengineering4040062>`_
     """
 
     def _sn(N_co_0, N_co2_0, N_h2_0):
         """"Stoichiometric number" of the initial conditions.
         """
 
         return (N_h2_0 - N_co2_0)/(N_co_0 + N_co2_0)
@@ -99,15 +99,15 @@
     xi_3 = xi[1]  # conversion of initial carbon dioxide to methanol
 
     return N_co, N_co2, N_h2, N_h2o, N_ch3oh, xi_3
 
 
 def plug_flow(mass_co_in, mass_co2_in, mass_h2_in, P=60, T=270, rho_catalyst=1000, n_tubes=10000, d_tubes=0.02, L_tubes=3, outflow='mass', output=None):
     """
-    Plug Flow Reactor (PFR) steady state flow simulation of hydrogenation of carbon dioxide to produce methanol with a Cu/ZnO/Al:sub:`2`O:sub:`3` catalyst.
+    Plug Flow Reactor (PFR) steady state flow simulation of hydrogenation of carbon dioxide to produce methanol with a Cu/ZnO/Al$_2$O$_3$ catalyst[1]_.
     
     Parameters
     ----------
     mass_co_in : float
         Mass flow rate in of carbon monoxide; kilograms per second.
     mass_co2_in : float
         Mass flow rate in of carbon dioxide; kilograms per second.
@@ -149,16 +149,15 @@
 
     Notes
     -----
     For `output = 'volume'`, it is assumed the outflow temperature is cool enough for the water and methanol to condense.
 
     References
     ----------
-    .. [1] J. Terreni, A. Borgschulte, M. Hillestad, and B. Patterson, "Understanding Catalysis-A Simplified Simulation of Catalytic Reactors for CO:sub:`2` Reduction," ChemEngineering, vol. 4, 2020.
-
+    .. [1] `J. Terreni, A. Borgschulte, M. Hillestad, and B. Patterson, "Understanding Catalysis-A Simplified Simulation of Catalytic Reactors for CO$_2$ Reduction," ChemEngineering, vol. 4, 2020.<https://doi.org/10.3390/chemengineering4040062>`_
     """
 
     def _kinetic_factors(a, b, T):
         """Kinetic factors in Arrhenius form.
         """
         return a * np.exp(b/(_constants.R*T))
```

### Comparing `pyseafuel-0.1.1/pyseafuel/system.py` & `pyseafuel-0.1.2/pyseafuel/system.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 import pyseafuel
 import pyseafuel._constants as _constants
 
 # ──────────────────────────────────────────────────────────────────────────
 
-# def seafuel(sea_water_carbon_dioxide_arm_flow, sea_water_hydrogen_arm_flow, water_ratio, stages, salt_removal, psu, sst, P, T, E0, K, r, A):
-# def seafuel(seawater_volume_in_degasser, seawater_volume_in_desalinator, seawater_S, seawater_T, desal_water_ratio, desal_stages, desal_salt_removal, electro_E0, electro_K, electro_R, electro_A, reactor_P, reactor_T, reactor_outflow):
 def seafuel(degasser, desalinator, electrolyzer, reactor):
     """
 
     Parameters
     ----------
     degasser : dict
         Degasser information; must contain the 'type' key. 'type' can equal on of the following: 'bipolar_membrane'.
         'bipolar_membrane' requires 'seawater_in' (seawater inflow) in L/s.
     desalintor : dict
         Desalinator information; must contain the 'type' key. 'type' can equal on of the following: 'electrodialysis'.
         'electrodialysis' requires 'seawater_in' (seawater inflow) in L/s, 'seawater_S' (seawater salinity) in PSU, 'seawater_T' (seawater temperature) in Kelvin, 'water_ratio' (volume ratio of fresh water out over seawater in) from (0, 1), 'salt_removal' (fraction of salt removed from the fresh water outflow) from (0, 1), and 'stages' (number of separation stages).
     electrolyzer : dict
         Electrolyzer information; must contain the 'type' key. 'type' can equal on of the following: 'Shen'.
-        'Shen' requires 'E0' (reversible cell potential) in V, 'K' (Shen et al. model power coeffecient) in ohm:sup:`-1` cm:sup:`-2`, 'R' (internal cell resistance) in ohm:sup:`1` cm:sup:`2`, and 'area' (area of the membrane stack) in cm:sup:`2`.
+        'Shen' requires 'E0' (reversible cell potential) in V, 'K' (Shen et al. 2011 model power coeffecient) in ohm$^{-1}$cm$^{-2}$, 'R' (internal cell resistance) in ohm$^1$cm$^2$, and 'area' (area of the membrane stack) in cm$^2$.
     reactor : dict
         Reactor information; must contain the 'type' key. 'type' can equal on of the following: 'plug_flow_reactor'.
         'plug_flow' requires 'P' (operating pressure of the reactor) in bars and 'T' (operating temperature of the reactor) in Celsius.
 
     Returns
     -------
     flows : dict
@@ -31,23 +29,23 @@
         Power consumption for each component, and total consumption.
     misc : dict
         Remaining useful non-flow, non-power related information.
 
     Notes
     -----
     For the input dictionaries, the 'type' value is derived from the function names found in the component's respective submodule.
+    """
 
-    The flow diagram for this system follows:
+    # The flow diagram for this system follows:
 
-    .. image:: ../diagrams/seafuel.png
+    # .. image:: ../diagrams/seafuel.png
 
-    Examples
-    --------
+    # Examples
+    # --------
 
-    """
 
     # degasser
     if degasser['type'] == 'bipolar_membrane':
         mass_co2_out, power_degas = pyseafuel.degasser.bipolar_membrane(degasser['seawater_in'])
         # mass_co2_out; kg/s
         # power_degas; W
```

### Comparing `pyseafuel-0.1.1/setup.py` & `pyseafuel-0.1.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 {'': ['*']}
 
 install_requires = \
 ['numpy>=1.21.1,<2.0.0', 'pdoc>=12.0.2,<13.0.0', 'scipy>=1.7.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'pyseafuel',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'Package to numerically model a methanol producing island.',
     'long_description': None,
     'author': 'Doug Keller',
     'author_email': 'dg.kllr.jr@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.9,<3.10',
+    'python_requires': '>=3.9',
 }
 
 
 setup(**setup_kwargs)
```

