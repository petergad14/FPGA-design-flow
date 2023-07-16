# FPGA design flow for Dummies by a Dummy
_If you are a beginner wanting to briefly know the FPGA design flow, you're in the right place. If you are a pro please leave :angry:_


> The flow is simple as shown in the figure below.

![FPGA design flow](https://github.com/petergad14/petergad14.github.io/assets/139645814/1505a23d-7371-45bd-8f28-c4fbf1f24739)

### Let's dig deep into each step.
1. `Functional specifications:` The process starts with defining the requirements and specifications of the desired circuit. This includes understanding the system-level functionality, input/output interfaces, performance requirements, and any specific constraints.
In this stage, the design can be written with C++, MATLAB, or Python codes.

2. `HDL:` In this step, a hardware description language (HDL) such as VHDL or Verilog is used to write the design description.
    * `Behavioral simulation:` The design is simulated and test vectors are applied to verify that the design functions correctly and meets the desired specifications.

3. `Synthesis:`The high-level design is then converted into Register-Transfer Level (RTL) code, which represents the design in terms of registers, logic blocks, and their interconnections. RTL synthesis tools map the high-level design to the target FPGA architecture, optimizing for factors such as performance, area, and power consumption as shown in the figure below.

<p align="center">
   <img src="https://github.com/petergad14/petergad14.github.io/assets/139645814/d8711fbf-e4b7-4402-a303-22c654816223" width="500" height="300">
</p>

4. `Place & Route:`The placement stage determines the physical location of each logic element within the FPGA chip, while the routing stage determines the interconnections between these elements.

   <p align="center">
   <img src="https://github.com/petergad14/petergad14.github.io/assets/139645814/2fe9c0d9-24df-4bc2-8ba3-1612f3c628e5" width="500" height="300">
   </p>

5. `STA:` After place and route, timing analysis is performed to ensure that the design meets the required timing constraints. This analysis considers factors such as signal delays, clock frequencies, and setup/hold times.


6. `Download and verify:`The FPGA is now programmed with the desired circuit functionality. This configures the FPGA with the desired circuit. The design is then verified and tested for correct functionality, performance, and compliance with the specifications.      
The design is then verified and tested for correct functionality, performance, and compliance with the specifications.
