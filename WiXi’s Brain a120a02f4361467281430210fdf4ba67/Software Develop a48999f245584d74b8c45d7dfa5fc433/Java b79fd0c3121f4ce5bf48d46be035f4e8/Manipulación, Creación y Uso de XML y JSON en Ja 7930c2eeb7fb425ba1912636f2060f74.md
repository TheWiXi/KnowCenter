# Manipulación, Creación y Uso de XML y JSON en Java

Propietario: William Meza
Verificación: Verificación vencida
Etiquetas: Java, advanced, intermediate

## 1. Introducción a XML y JSON

XML (Extensible Markup Language) y JSON (JavaScript Object Notation) son formatos de intercambio de datos comunes utilizados en el desarrollo de aplicaciones. Ambos ofrecen estructuras jerárquicas para representar datos de manera legible y eficiente. En Java, existen bibliotecas como JAXP (Java API for XML Processing) y Jackson que facilitan la manipulación, creación y uso de XML y JSON.

## 2. Manipulación de XML con JAXP

### 2.1 Lectura de un Documento XML

```java
import javax.xml.parsers.DocumentBuilder;
import javax.xml.parsers.DocumentBuilderFactory;
import org.w3c.dom.Document;
import org.w3c.dom.Element;
import org.w3c.dom.NodeList;

public class LeerXML {
    public static void main(String[] args) {
        try {
            DocumentBuilderFactory factory = DocumentBuilderFactory.newInstance();
            DocumentBuilder builder = factory.newDocumentBuilder();

            Document document = builder.parse("archivo.xml");

            NodeList nodeList = document.getElementsByTagName("elemento");

            for (int i = 0; i < nodeList.getLength(); i++) {
                Element element = (Element) nodeList.item(i);
                System.out.println("Contenido: " + element.getTextContent());
            }
        } catch (Exception e) {
            e.printStackTrace();
        }
    }
}

```

### 2.2 Escritura de un Documento XML

```java
import javax.xml.parsers.DocumentBuilder;
import javax.xml.parsers.DocumentBuilderFactory;
import javax.xml.transform.Transformer;
import javax.xml.transform.TransformerFactory;
import javax.xml.transform.dom.DOMSource;
import javax.xml.transform.stream.StreamResult;
import org.w3c.dom.Document;
import org.w3c.dom.Element;

public class EscribirXML {
    public static void main(String[] args) {
        try {
            DocumentBuilderFactory factory = DocumentBuilderFactory.newInstance();
            DocumentBuilder builder = factory.newDocumentBuilder();
            Document document = builder.newDocument();

            Element rootElement = document.createElement("root");
            document.appendChild(rootElement);

            Element elemento = document.createElement("elemento");
            elemento.appendChild(document.createTextNode("Contenido"));
            rootElement.appendChild(elemento);

            TransformerFactory transformerFactory = TransformerFactory.newInstance();
            Transformer transformer = transformerFactory.newTransformer();
            DOMSource source = new DOMSource(document);

            StreamResult result = new StreamResult("nuevoArchivo.xml");
            transformer.transform(source, result);
        } catch (Exception e) {
            e.printStackTrace();
        }
    }
}

```

## 3. Manipulación de JSON con Jackson

### 3.1 Lectura de un Documento JSON

```java
import com.fasterxml.jackson.databind.JsonNode;
import com.fasterxml.jackson.databind.ObjectMapper;

public class LeerJSON {
    public static void main(String[] args) {
        try {
            ObjectMapper mapper = new ObjectMapper();
            JsonNode rootNode = mapper.readTree("archivo.json");

            JsonNode nodoElemento = rootNode.get("elemento");

            String contenido = nodoElemento.asText();
            System.out.println("Contenido: " + contenido);
        } catch (Exception e) {
            e.printStackTrace();
        }
    }
}

```

### 3.2 Escritura de un Documento JSON

```java
import com.fasterxml.jackson.databind.ObjectMapper;
import com.fasterxml.jackson.databind.node.ObjectNode;

public class EscribirJSON {
    public static void main(String[] args) {
        try {
            ObjectMapper mapper = new ObjectMapper();
            ObjectNode rootNode = mapper.createObjectNode();

            rootNode.put("elemento", "Contenido");

            mapper.writeValue(new File("nuevoArchivo.json"), rootNode);
        } catch (Exception e) {
            e.printStackTrace();
        }
    }
}

```

## 4. Conclusiones

La manipulación, creación y uso de XML y JSON en Java es esencial para el intercambio de datos entre aplicaciones. Las bibliotecas como JAXP y Jackson facilitan estas tareas, proporcionando métodos simples para leer y escribir archivos en ambos formatos. Estas habilidades son fundamentales para el desarrollo de aplicaciones que necesitan interoperar con sistemas externos o compartir información de manera estructurada. ¡Explora y utiliza estas capacidades para mejorar el manejo de datos en tus aplicaciones Java!