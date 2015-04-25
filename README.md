# Lua

Configures and installs Lua related software

## Requirements

- Ansible 1.2+
- Ubuntu 12.04+


## Variables

### Lua

| Name                      | Default  | Description                                                       |
|---------------------------|----------|-------------------------------------------------------------------|
| `lua_install_method`      | package  | Lua installation method (source or package)                       |
| `lua_package_name`        | lua5.2   | Lua package name to install when installing as a package          |
| `lua_source_version`      | 5.2.3    | Lua version to install when installing from source                |
| `luarocks_install_method` | package  | The LuaRocks installation method (source or package)              |
| `luarocks_package_name`   | luarocks | The LuaRocks package name to install when installing as a package |
| `luarocks_source_version` | 2.1.2    | The LuaRocks version to install when installing from source       |
| `luajit_install_method`   | package  | The LuaJIT installation method (source or package)                |
| `luajit_package_name`     | luajit   | The package name to install when installing as a package          |
| `luajit_source_version`   | 2.0.2    | The version to install when installing from source                |


Dependencies
------------

None


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: mattupstate.lua, lua_install_method: source }

License
-------

MIT

Author Information
------------------

Matt Wright <matt@nobien.net>
