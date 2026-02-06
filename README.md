# ⌨️ My Glove80 ZMK Config

This repository contains my personal keyboard layout for the **MoErgo Glove80**. It is specifically optimized for **Java development**, emphasizing efficient access to symbols and numbers through a mix of momentary layers and home-row combos.

## 🚀 Layout Strategy

The goal of this layout is to minimize hand movement and "finger gymnastics" when writing verbose Java code.

### 1. The Symbol Layer (Lower)
* **Access:** Momentary Hold (`&mo`) on the Left Thumb.
* **Logic:** Designed for "chording." Hold with the thumb while the right hand strikes brackets `()`, braces `{}`, and operators `->`.
* **Transparency:** Thumb keys and Modifiers are set to `&trans` to allow for `Shift + Symbol` combinations.

### 2. The Number Layer
* **Access:** Home-row Combo `J + K`.
* **Behavior:** Toggle (`&tog`). 
* **Use Case:** Best for heavy data entry, array indexing, or constants where staying in the layer is more efficient than holding a key.

### 3. Navigation & Magic
* **Magic Layer:** Accessed via the dedicated Magic key. Used for Bluetooth profile switching and entering the **Bootloader**.
* **Safety:** Every layer contains a "Panic Button" shortcut to `&to 0` to ensure I never get trapped in a sub-layer.

## 🛠 Features

| Feature | Description |
| :--- | :--- |
| **Combos** | `D + F` (Symbols) and `J + K` (Numbers). Set to **Global** scope. |
| **Sticky Keys** | `&sl` used for single-character injections to maintain typing flow. |
| **Auto-Pairing** | Macros for `()` and `{}` that automatically move the cursor inside. |


## 🔄 Workflow

Since I am using the **File System** editing method with the Nick Coutsos editor, the update process is as follows:

1. **Edit:** Open the [Keymap Editor](https://nickcoutsos.github.io/keymap-editor/) and modify the local `.keymap` file.
2. **Commit:**
   ```bash
   git add .
   git commit -m "feat: optimized bracket macros for Java"
   git push origin main
