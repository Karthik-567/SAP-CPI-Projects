# Employee Data Integration

## Objective

Retrieve employee data from a REST API and send it to another system after transforming XML to JSON.

---

## Scenario

A company stores employee information in XML format.

SAP CPI receives the XML, transforms it into JSON, and sends it to the target application.

---

## Components Used

- HTTPS Sender
- Content Modifier
- Message Mapping
- Groovy Script
- XML to JSON Converter
- HTTPS Receiver

---

## Flow

HTTPS Sender
↓

Content Modifier
↓

Message Mapping
↓

Groovy Script
↓

XML to JSON Converter
↓

HTTPS Receiver

---

## Input Payload

```xml
<Employee>
    <ID>101</ID>
    <Name>Karthik</Name>
    <Department>IT</Department>
</Employee>
```

## Output Payload

```json
{
  "id":101,
  "name":"Karthik",
  "department":"IT"
}
```

## Status

✅ Completed
