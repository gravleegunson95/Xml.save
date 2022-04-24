# Xml.save
Local $oXML = ObjCreate("Microsoft.XMLDOM") $oXML.load("ConEmu.xml") Local $oNode = $oXML.SelectSingleNode("//value[@name='AnsiLogPath']") ConsoleWrite($oNode.xml &amp; @CRLF) $oNode.setAttribute("data", "testpath") ConsoleWrite($oNode.xml &amp; @CRLF) $oXml.save("NewConEmu.xml"
