# Cave Programming language

go to : cavewebsite.onredner.com for more info

## Syntaxes

to print on the console use the following, 

* write("Hello World!!")
* write(variable_name)
* write(&red, "Colored text!") || options: &red, &green, &blue, &yellow
* write(_) || Clears the terminal screen
* scan(!var, "Enter value: ") || Prompts for user input

Note: Strings support escape sequences like `\n` and `\t`.

We can also wait for some time. 

* wait(ms)
* pause || Waits for any key press to continue
* os("clear") || Executes a system OS command

Note: this only works with "Milliseconds"

1 second = 1000 ms

to declare a variable use the following, 

* !variable_name = intvalue
* ?variable_name = floatvalue
* @variable_name = stringvalue

to use if-else use the following, 

* #if (variable_name == value) {
    
}
* #elseif (variable_name == value) {
    
}
* #else {
    
}

"#" is for logic statements
and, or, nand, nor, xor, xnor, not, == are used for condition type statements

for conditional loops use the following

* #while(condition) {
    
}

for loops without a condition use the following

* #loop {
    
}

for repeating use this

* #turn (number of times to repeat) {
    
}

for range loops use this

* #for (!i in r(end_value)) {
    write(!i)
}

to declare a function use the following

* function function_name(var1; var2; var3; and so on) {
    write(var1)
}

to call the function use this

* get function_name(value1; value2; value3; and so on)

to use lists do this

* list_name = ()

to use tuples do this

* tuple_name = []

to use a dictionary use this

* dict_name = {}

We can * list_name.append(), list_name.goto(), list_name.length(), list_name.delete(), list_name.cancel(),
list_name.from(starting_val, ending_val)

to use file use this

*file.run(filename), file.edit(filename, contentline), file.delete(filename), file.create(filename),
file.read(filename), file.see(filename)

Some values to set on and off are

* &0 = false/off
* &1 = true/on

to return a value do

return value

To include a library/plugin do

* #insert lib_name

* #cancel lib_name

* #inserted?("lib_name") || Returns 1 if loaded, 0 if not

## CLI Usage

Use the Cave CLI for managing your installation:

* cave cli install <plugin_name>  - Install a plugin from the repository
* cave cli update <plugin_name>   - Update an existing plugin
* cave cli remove <plugin_name>   - Uninstall a plugin

Comments, these are used to add notes to blocks, lines or something on a code

* || - Single line Comment
* /| - End line comment
* |\ - Start line comment

For more information on creating plugins, see: Doc/PLUGINS.md
