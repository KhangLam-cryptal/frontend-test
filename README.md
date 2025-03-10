# Frontend Developer Test - Web2 & Web3

## 📌 Overview
This test evaluates your frontend skills in building a **Web2 & Web3-integrated marketplace**. You will:
- Fetch and display business ideas from an API.
- Connect to **Metamask** using Web3.
- Implement a purchase function using a **smart contract**.

**🕒 Duration:** 4 hours  
**⚙️ Tech Stack:** Next.js, Tailwind CSS, Ethers.js, Axios

---

## 🎯 Requirements

### **1️⃣ Setup Development Environment**
Clone this repository and install dependencies:
```bash
 git clone <repository_url>
 cd frontend-test
 npm install
 npm run dev
```
Ensure you have **Metamask** installed.

### **2️⃣ Display Business Ideas (API - Web2)**
- Fetch ideas from `/api/ideas`.
- Show **title, description, price (ETH), owner**.
- Clicking an idea navigates to `/idea/[id]`.

📌 **Example API Response (`GET /api/ideas`)**:
```json
[
  {
    "id": "1",
    "title": "AI Startup Evaluator",
    "description": "AI-based startup assessment platform.",
    "price": "0.5",
    "owner": "0x1234...abcd"
  }
]
```

### **3️⃣ Connect Metamask (Web3)**
- Implement **wallet connection** using **ethers.js**.
- Display the connected address.
- Show the **"Buy Idea"** button only if connected.

📌 **Example Metamask Connection Code:**
```javascript
const provider = new ethers.providers.Web3Provider(window.ethereum);
await window.ethereum.request({ method: "eth_requestAccounts" });
const signer = provider.getSigner();
const address = await signer.getAddress();
```

### **4️⃣ Display Idea Details**
- Fetch idea details from `GET /api/ideas/:id`.
- Display **title, description, price, owner**.
- If Metamask is connected, show the **Buy Idea** button.

### **5️⃣ Web3 Integration: Purchase Idea via Smart Contract**
- Call smart contract to process payment.

📌 **Example Contract (`IdeaMarketplace.sol`)**:
```solidity
contract IdeaMarketplace {
    function buyIdea(uint256 ideaId) public payable {}
}
```

📌 **Ethers.js Purchase Function:**
```javascript
const contract = new ethers.Contract(contractAddress, contractABI, signer);
await contract.buyIdea(ideaId, { value: ethers.utils.parseEther(price) });
```

---

## 📊 Evaluation Criteria
| Criteria | Points |
|----------|--------|
| Correct API implementation | 20 |
| Responsive & clean UI (Tailwind CSS) | 20 |
| Metamask connection & wallet display | 20 |
| Smart contract purchase function | 20 |
| Code quality & readability | 20 |
| **Total** | **100** |

---

## 📌 Submission Guidelines
Submit:
✅ GitHub repository link  
✅ A short demo video  
✅ README.md explaining setup & features  

**🚀 Good luck!**
