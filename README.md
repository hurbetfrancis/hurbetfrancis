using System.Collections.Generic;
using static System.Runtime.InteropServices.JavaScript.JSType;

--this is an example for the script, use this to make your own!(Might be adding custom Themes)
local Lib = loadstring(game: HttpGet("https://raw.githubusercontent.com/7yhx/kwargs_Ui_Library/main/source.lua"))()

local UI = Lib:Create{
    Theme = "Dark", --or any other theme
    Size = UDim2.new(0, 555, 0, 400)-- default
}

local Main = UI:Tab{
   Name = "Inicio"
}

local Divider = Main:Divider{
   Name = "Inicio shit"
}

local QuitDivider = Main:Divider{
   Name = "Sair"
}
--This script requires a Lua client and server, as well as a secure connection between them.
local function createClient() 
    local host = "127.0.0.1" -- Replace with your server's IP address or domain name
    local port = 55555 -- Replace with your server's port number
    
    local sock = nil 
    local ok, err = tcp.connect(sock, host, port) 
     if not ok then return nil, ("Could not connect to the server: %s"):format(err) end-- Check for errors in connecting to the server   sock:settimeout(3000)-- Set timeout to 3 seconds for reading from the socket   return sock   end                       -- Function to create a Lua client object (LuaSocket library is required)                        --------------------------------------------------------------                        ----- ESP code goes here -----                        --------------------------------------------------------------```
