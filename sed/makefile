



TARGETS = test111 test112 test113 test114 test103 test104


# Define variables for clarity (assuming sim_vcs_system is the common path)
SIM_DIR = sim_vcs_system



SED_CMD2 = sed -e 's/^\/\/`define\s*SYSTEM_"$$dir"\s*1/`define SYSTEM_"$$dir" 1/' system/top_bench.sv
SED_CMD = sed -e 's|^//`define\s*SYSTEM_"$$dir"\s*1|`define SYSTEM_"$$dir" 1|' system/top_bench.sv

.PHONY: setup_sed
setup_sed:
	for dir in $(TARGETS); do \
        $(SED_CMD) > $(SIM_DIR)_$$dir/top_bench.sv; \
    done

.PHONY: setup
setup:
	rm -rf sim_vcs_system_test111
	cp -r system sim_vcs_system_test111
	sed -e 's/^\/\/`define\s*SYSTEM_test111\s*1/`define SYSTEM_test111 1/' system/top_bench.sv > sim_vcs_system_test111/top_bench.sv
	
	rm -rf sim_vcs_system_test112
	cp -r system sim_vcs_system_test112
	sed -e 's/^\/\/`define\s*SYSTEM_test112\s*1/`define SYSTEM_test112 1/' system/top_bench.sv > sim_vcs_system_test112/top_bench.sv
	
	rm -rf sim_vcs_system_test103
	cp -r system sim_vcs_system_test103
	sed -e 's/^\/\/`define\s*SYSTEM_test103\s*1/`define SYSTEM_test103 1/' system/top_bench.sv > sim_vcs_system_test103/top_bench.sv
	
	rm -rf sim_vcs_system_test104
	cp -r system sim_vcs_system_test104
	sed -e 's/^\/\/`define\s*SYSTEM_test104\s*1/`define SYSTEM_test104 1/' system/top_bench.sv > sim_vcs_system_test104/top_bench.sv
	
	rm -rf sim_vcs_system_test113
	cp -r system sim_vcs_system_test113
	sed -e 's/^\/\/`define\s*SYSTEM_test113\s*1/`define SYSTEM_test113 1/' system/top_bench.sv > sim_vcs_system_test113/top_bench.sv
	
	rm -rf sim_vcs_system_test114
	cp -r system sim_vcs_system_test114
	sed -e 's/^\/\/`define\s*SYSTEM_test114\s*1/`define SYSTEM_test114 1/' system/top_bench.sv > sim_vcs_system_test114/top_bench.sv


