# Testconst avatar = {
  hair: "brown",
  eyes: "blue",
  skin: "light",
  clothes: "t-shirt",
  accessory: "glasses"
};

function generateAvatar() {
  // Generate random avatar properties
  const hairColors = ["brown", "blonde", "black", "red"];
  const eyesColors = ["blue", "green", "brown"];
  const skinColors = ["light", "medium", "dark"];
  const clothesStyles = ["t-shirt", "sweater", "shirt"];
  const accessories = ["hat", "glasses", "necklace"];

  avatar.hair = hairColors[Math.floor(Math.random() * hairColors.length)];
  avatar.eyes = eyesColors[Math.floor(Math.random() * eyesColors.length)];
  avatar.skin = skinColors[Math.floor(Math.random() * skinColors.length)];
  avatar.clothes = clothesStyles[Math.floor(Math.random() * clothesStyles.length)];
  avatar.accessory = accessories[Math.floor(Math.random() * accessories.length)];

  // Display the avatar on the website
  const avatarContainer = document.querySelector("#avatar");
  avatarContainer.innerHTML = <img src="avatars/${avatar.hair}_${avatar.eyes}_${avatar.skin}_${avatar.clothes}_${avatar.accessory}.svg">;
}

