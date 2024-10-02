requires a include/GLFW folder to include/*.h when you build GLFW
also you need the glfw3.dll in the root folder and glfw lib in the lib folder

test

args for the task.json for the compiler:

[
"-g",
"-I${workspaceFolder}/include",
"-L${workspaceFolder}/lib",
"${workspaceFolder}/src/*.cpp",
"${workspaceFolder}/src/glad.c",
"-lglfw3dll",
"-lopengl32",
"-o",
"${workspaceFolder}/build/main.exe"
]