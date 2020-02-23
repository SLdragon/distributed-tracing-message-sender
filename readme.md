## How to build this sample


1. Install ["Desktop development with C++" workload](https://docs.microsoft.com/cpp/build/vscpp-step-0-installation?view=vs-2019) for Visual Studio 2019. Visual Studio 2017 and 2015 are also supported.

1. Install [CMake](https://cmake.org/). Make sure it is in your `PATH` by typing `cmake -version` from a command prompt.

1. Use the command below to build the iothub_ll_telemetry_sample project

    ```cmd
    git clone https://github.com/SLdragon/distributed-tracing-message-sender.git
    cd distributed-tracing-message-sender
    git submodule update --init

    mkdir cmake
    cd cmake
    cmake ..

    cd iothub_client/samples/iothub_ll_telemetry_sample
    cmake --build . --target iothub_ll_telemetry_sample --config Release
    ```

1. Then you can find the binary in the here:

    ```
    distributed-tracing-message-sender\cmake\iothub_client\samples\iothub_ll_telemetry_sample\Release\iothub_ll_telemetry_sample.exe
    ```

## How to use this binary
    ```
    iothub_ll_telemetry_sample.exe [Your_Device_Connection_String]
    ```
