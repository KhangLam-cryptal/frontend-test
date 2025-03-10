**BÀI TEST FRONTEND - WEB2 & WEB3 & BLOCKCHAIN**

---

### **1. Mô tả bài test**
Bài test dành cho ứng viên frontend nhằm đánh giá kỹ năng lắp trình Web2 & Web3, bao gồm:
- Xây dựng UI theo thiết kế cho Web2.
- Kết nối API backend.
- Tương tác với MetaMask và blockchain.
- Hiển thị dữ liệu từ smart contract.

---

### **2. Yêu cầu chung**
- **Ngôn ngữ:** TypeScript + React.js (Next.js được khuyến khích).
- **UI framework:** TailwindCSS / Chakra UI / Ant Design.
- **Quản lý state:** React Context / Redux Toolkit.
- **API backend:** Gọi API RESTful hoặc GraphQL.
- **Kết nối Web3:** ethers.js / web3.js.
- **Blockchain:** Ethereum / Polygon (EVM-compatible).
- **Smart contract:** ERC-721 hoặc ERC-1155 NFT contract (có sẵn).

---

### **3. Bài test chi tiết**
#### **Phần 1: Xây dựng giao diện Web2**
- Thiết kế giao diện theo file Figma (sẽ gửi sau khi đăng ký test).
- Bao gồm các trang:
  1. **Trang chính**: Hiển thị danh sách sản phẩm (gọi API backend).
  2. **Trang chi tiết**: Hiển thị chi tiết sản phẩm.
  3. **Trang user profile**: Hiển thị thông tin user (đã đăng nhập).
- Yêu cầu responsive.

#### **Phần 2: Kết nối API backend**
- Gọi API lấy danh sách sản phẩm, chi tiết sản phẩm.
- Sử dụng fetch API / axios.
- Hiển thị loading khi API chưa tải xong.

#### **Phần 3: Kết nối Web3 - MetaMask**
- Nút "Connect Wallet" kết nối với MetaMask.
- Hiển thị địa chỉ ví của user sau khi kết nối.
- Kiểm tra xem user đang dùng network Ethereum hay Polygon, nếu sai thì hiển thị thông báo.

#### **Phần 4: Hiển thị dữ liệu từ Blockchain**
- Hiển thị danh sách NFT từ smart contract (contract có sẵn).
- Hiển thị metadata NFT (tên, hình ảnh, mô tả) lấy từ IPFS hoặc URL trong contract.
- Sử dụng ethers.js để gọi contract methods.

#### **Phần 5: Chức năng mua NFT (để test, không dùng tiền thật)**
- Nút "Mua" (giả định NFT có giá 0.01 ETH testnet).
- Gửi giao dịch mua NFT tới smart contract.
- Hiển thị transaction hash sau khi giao dịch thành công.

---

### **4. Cách thức nộp bài**
- Fork repo test trên GitHub và commit code lên repo cá nhân.
- Gửi link repo cùng file video quay lại quá trình chạy demo.
- Sử dụng testnet (Goerli / Mumbai) để test giao dịch blockchain.

---

### **5. Tiêu chí đánh giá**
- **Hoàn thiện UI** (30%): Layout đúng thiết kế, UI/UX tốt, responsive.
- **Tốc độ và performance** (20%): Tối ưu tốc độ, code sạch, dễ bảo trì.
- **API và Web3** (30%): Kết nối backend, MetaMask, blockchain chuẩn.
- **Tính sáng tạo & tự học hỏi** (20%): Tính logic và sáng tạo trong code.

---

### **6. Hỗ trợ**
- Trong quá trình làm bài, nếu có thắc mắc, vui lòng liên hệ qua email/Zalo/Telegram của người phụ trách.

---

Chúc bạn làm bài tốt! 🚀

