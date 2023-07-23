# NOTE: on MacOS you need to add an addition flag: -undefined dynamic_lookup

# To compile the .cpp file from the basic example provided by pybind11 official website:
#
# INCLUDE = -I/Users/zionsheng/miniconda3/lib/python3.10/site-packages/pybind11/include/ -I/Users/zionsheng/miniconda3/include/python3.10/
# default:
# 	c++ -O3 -Wall -shared -std=c++11 -fPIC -undefined dynamic_lookup $(INCLUDE) src/example.cpp -o src/example.so

INCLUDE = -I/Users/zionsheng/miniconda3/lib/python3.10/site-packages/pybind11/include/ -I/Users/zionsheng/miniconda3/include/python3.10/
FLAG = -O3 -Wall -Werror -shared -std=c++11 -fPIC -undefined dynamic_lookup
default:
	c++ $(FLAG) $(INCLUDE) $(python3 -m pybind11 --includes) src/simple_ml_ext.cpp -o src/simple_ml_ext.so
