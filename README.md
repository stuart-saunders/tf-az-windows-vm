# Azure Windows VM Module

Usage:-
```
module "windows-vm" {
  source  = "./modules/windows-vm"
  vm_name = "windows-vm"

  ip_configuration_name = var.ip_configuration_name
  subnet_id             = azurerm_subnet.this.id
  location              = azurerm_resource_group.this.location
  resource_group_name   = azurerm_resource_group.this.name
}
```
