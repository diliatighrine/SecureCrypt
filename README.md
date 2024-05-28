# SecureCrypt
SecureCrypt est une bibliothèque Node.js qui offre un chiffrement et un déchiffrement robustes pour sécuriser vos données sensibles. Basée sur l'algorithme AES-256-CBC

cette bibliothèque utilise une clé de chiffrement de 256 bits pour garantir un niveau élevé de sécurité. Les fonctions d'encryption et de decryption sont optimisées pour assurer des performances maximales tout en préservant l'intégrité des données. Que vous développiez une application web, mobile ou desktop, SecureCrypt vous fournit une solution fiable pour protéger vos informations confidentielles. Intégrez SecureCrypt dans vos projets dès aujourd'hui pour renforcer la sécurité de vos données.

Installation:

npm install secure-crypt

Utilisation

javascript

const secureCrypt = require('secure-crypt');

// Définir votre clé de chiffrement (doit être de 256 bits)
const ENCRYPTION_KEY = process.env.ENCRYPTION_KEY;

// Encrypter une chaîne de caractères
const encryptedText = secureCrypt.encrypt('Texte confidentiel à chiffrer', ENCRYPTION_KEY);

// Décrypter une chaîne de caractères
const decryptedText = secureCrypt.decrypt(encryptedText, ENCRYPTION_KEY);

console.log('Texte chiffré:', encryptedText);
console.log('Texte déchiffré:', decryptedText);

Fonctions
encrypt(text: string, key: string): string

Cette fonction prend une chaîne de caractères text et une clé de chiffrement key en entrée, et retourne la chaîne de caractères chiffrée.
decrypt(text: string, key: string): string

Cette fonction prend une chaîne de caractères chiffrée text et une clé de chiffrement key en entrée, et retourne la chaîne de caractères déchiffrée.
