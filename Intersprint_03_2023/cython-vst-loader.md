# cython-vst-loader short documentation

Cython-vst-loader is a Python package that provides a simple and efficient way to load VST plugins into Python applications. It is based on the Cython language, which is a superset of Python that allows for fast and efficient execution of code.

To use cython-vst-loader, you first need to install the package using pip:

```pip install cython-vst-loader```

Once the package is installed, you can load a VST plugin using the following code:

```
from cython_vst_loader import VSTPlugin

plugin = VSTPlugin("path/to/plugin.dll")
plugin.open()
```

This will load the VST plugin located at the specified path and open it for use. You can then use the **plugin** object to interact with the plugin and its parameters.

Here are some of the methods available on the VSTPlugin object:

**process(inputs, outputs, block_size)**: Processes audio data for the plugin. **inputs** and **outputs** are numpy arrays representing the audio input and output buffers, and **block_size** is the number of audio samples to process at a time.

**set_parameter(index, value)**: Sets the value of a plugin parameter. **index** is the index of the parameter, and **value** is the new value.

**get_parameter(index)**: Gets the current value of a plugin parameter. **index** is the index of the parameter.

**get_parameter_name(index)**: Gets the name of a plugin parameter. **index** is the index of the parameter.

**get_parameter_count()**: Gets the number of parameters on the plugin.

**close()**: Closes the plugin and frees its resources.

That's the basic overview of the cython-vst-loader package. With this package, you can easily incorporate VST plugins into your Python applications and manipulate them as needed.