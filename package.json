const express = require("express");
const path = require("path");
const app = express();

app.use(express.static(__dirname));

// Default route → scan.html
app.get("/", (req, res) => {
  res.sendFile(path.join(__dirname, "scan.html"));
});

// Render requires this to start on the right port
const PORT = process.env.PORT || 3000;
app.listen(PORT, () => console.log("Server running on port " + PORT));
