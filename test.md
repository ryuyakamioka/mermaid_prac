```mermaid
sequenceDiagram
    actor Alice
    participant Source 1
    participant Source 2
    participant Service A
    participant Database A

    Alice->>Source 1: 情報1取得
    Source 1->>Alice: 
    Alice->>Source 2: 情報2取得
    Source 2->>Alice: 
    Alice->>Alice: 結果=情報1+情報2
    Alice->>Service A: 結果格納
    Service A->>Database A: 結果格納
```