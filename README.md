# esp32-setup
esp32 setup notes


    if(EXISTS "${CMAKE_SOURCE_DIR}/fix_compile_commands.py")
        add_custom_target(
            fix_clangd ALL
            COMMAND ${CMAKE_COMMAND} -E echo "Running fix_compile_commands.py..."
            COMMAND ${CMAKE_COMMAND} -E env python3 ${CMAKE_SOURCE_DIR}/fix_compile_commands.py
            COMMENT "Cleaning compile_commands.json for clangd"
            VERBATIM
        )
    endif()


5.5.4 with vscode extension prblem 
$env_var_pairs = @{
    "IDF_TOOLS_PATH" = "C:\Espressif\tools"
    "IDF_COMPONENT_LOCAL_STORAGE_URL" = "file://C:\Espressif\tools"
    "IDF_PATH" = "C:\esp\v5.5.4\esp-idf"
    "OPENOCD_SCRIPTS" = "C:\Espressif\tools\openocd-esp32\v0.12.0-esp32-20251215/openocd-esp32/share/openocd/scripts"
    "IDF_CCACHE_ENABLE" = "1"
    "ESP_ROM_ELF_DIR" = "C:\Espressif\tools\esp-rom-elfs\20241011/"
    "IDF_PYTHON_ENV_PATH" = "C:\Espressif\tools\python\v5.5.4\venv"
}

missing some items in file "C:\Espressif\tools\Microsoft.v5.5.4.PowerShell_profile.ps1"