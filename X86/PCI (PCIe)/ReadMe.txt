
PCIe在PCI总线技术上发展而来。在驱动程序上PCIe兼容PCI的驱动程序。如果你是PCI/PCIe的初学开发者，你应当首先参考学习PCI的相关文档，
因为PCIe的配置空间是基于PCI配置空间扩展而来的。PCIe的官方规格书中只介绍了新增特性部分，兼容部分（包括寄存器位段等内容）需要参考PCI
官方规格书、“PCI Bridge to Bridge” 规格书 和 “CardBus” 规格书等。

注：在PCIe规范中，明确要求PCIe设备必须支持 MSI / MSI-X机制。 但是，由于PCIe可以模拟PCi的INTx机制，因此实际PCIe设备不实现MSI/MSI-X
也可以实现中断触发，实际上这类芯片的确存在，例如：沁恒 WCH382 ...  (被坑惨了...!)
