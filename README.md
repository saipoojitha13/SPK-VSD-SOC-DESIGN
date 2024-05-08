# SPK-VSD-SOC-DESIGN

NASSCOM-VSD-SOC-DESIGN-PROGRAM

CONTENTS:
  DAY1: Inception of Open-source EDA, OpenLANE and Sky130 PDK
  
            > 1.How to talk to computers ?
                

            
              >> introduction to QFN-48 Package, chip, pads, core, die and IPs:
              This is arduino Leonardo board and the highlighted part is the chip. the chip is designed from RTL TO GDS Flow pipeline
                
  ![image](https://github.com/saipoojitha13/SPK-VSD-SOC-DESIGN/assets/142095120/91009dd7-6177-4af6-bfc5-ccd81010d9c3)

            
              >> introduction to RISC-V
              >> From Software applications to Hardware
              
            > SOC Design and OpenLane
              >> Introduction to all components of Open-Source digital ASIC design 
              >> Simplified RTL2GDS Flow
              >> Introduction to OpenLane and Strive chipsets
              >> Introduction to OpenLane detailed ASIC design flow

            > Get Familiar to Open-Source EDA tools
              >> OpenLane Directory Structure in Detail
              >> Design Preparation step
              >> Review files after design preparation and run synthesis
              >> OpenLane project Gitlink description
              >> steps to characterize synthesis results


DAY1:  we have to start our lab with the following commands:
      cd Desktop,
      cd work/tools/openlane_working_dir/openlane,
      docker ./flow.tcl -interactive.             
                ![1](https://github.com/saipoojitha13/SPK-VSD-SOC-DESIGN/assets/142095120/42e894c3-7c13-464a-b7d0-aa8ad5e384e1)
                now we use the following commands to run the synthesis:
      % package require openlane 0.9,
      % prep -design picorv32a,
      % run synthesis: here synthesis command will do the synthesis process and outputs the result as 
      ![1 6](https://github.com/saipoojitha13/SPK-VSD-SOC-DESIGN/assets/142095120/42d7e47b-fb92-4dde-a3c8-21197e60e2d7)
      now to observe the output we run following few commands on the new tab:
      cd work/tools/openlane_working_dir/openlane/designs/picorv32a/runs/08-05_04-23/reports/synthesis
      **less 1-yosys_4.stat.rpt:**
      ![1 4](https://github.com/saipoojitha13/SPK-VSD-SOC-DESIGN/assets/142095120/491f9bef-cbbc-4c10-bd98-c6e8b8b8708c)
      ![1 4 1](https://github.com/saipoojitha13/SPK-VSD-SOC-DESIGN/assets/142095120/9e5fedaf-547a-432b-979d-4d20e2c2699d)
      **less 2-opensta.timing.rpt:**  
      ![Screenshot from 2024-05-08 12-22-09](https://github.com/saipoojitha13/SPK-VSD-SOC-DESIGN/assets/142095120/6216a6a5-b8b0-4c93-9015-6dff849e3995)
      ![Screenshot from 2024-05-08 12-22-16](https://github.com/saipoojitha13/SPK-VSD-SOC-DESIGN/assets/142095120/f9b55d59-02c3-4025-955c-5fb50fcd27d3)


      
      
      

    
  
  
                      
