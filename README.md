# Blockstate-Reader
A Minecraft data pack for reading blockstates to an NBT storage.

## Features
- Read all blockstates of a block to an NBT storage
- Read individual blockstates of a block to an NBT storage
- Provides block tags for every blockstate

## Usage
To read blockstates of a block you need to run the function **at the location of the block you want to check**.
### Read all blockstates of a block
Run the function `blockstate:store/all`. 
This will clear **all** stored blockstate data. To preserve data run `blockstate:store/all_noclear` instead.
### Read specific blockstate of a block
Run function in `blockstate:store` corresponding to the blockstate you want to check for.   
Example: `function blockstate:store/waterlogged` will read only the `waterlogged` data of the block and clear `read.waterlogged` if there is none
### Access read blockstate data
All read data is stored in the data storage `blockstate:data` in the `read` tag.   
To view all blockstate data run `/data get storage blockstate:data read`   
Blockstates are stored in individual tags such as `read.power`.
### Clear storage
To clear stored blockstate data run the function `blockstate:clear`
### Check if block has blockstate
All blockstates have their own tag under the `blockstate` namespace.   
Using this you can for example check if a block has the `facing` blockstate: `execute if block ~ ~ ~ #blockstate:facing`
