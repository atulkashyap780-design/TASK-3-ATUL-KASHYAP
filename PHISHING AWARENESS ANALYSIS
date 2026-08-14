# ============================================
# Cyber Security Project 3
# Phishing Awareness Analysis
# ============================================

cat("\n============================================\n")
cat("       PHISHING AWARENESS ANALYZER\n")
cat("============================================\n\n")

# Take message from user
message <- readline("Enter the email/message to analyze: ")

# Convert message to lowercase
text <- tolower(message)

# Suspicious keywords
phishing_keywords <- c(
  "urgent",
  "verify",
  "password",
  "account blocked",
  "account suspended",
  "click here",
  "confirm",
  "login",
  "winner",
  "prize",
  "claim",
  "security alert"
)

# Store red flags
red_flags <- character(0)

# Check suspicious keywords
for (keyword in phishing_keywords) {
  if (grepl(keyword, text, fixed = TRUE)) {
    red_flags <- c(
      red_flags,
      paste("Suspicious keyword:", keyword)
    )
  }
}

# Check for links
if (grepl("https?://|www\\.", text)) {
  red_flags <- c(red_flags, "Message contains a link")
}

# Check for HTTP
if (grepl("http://", text, fixed = TRUE)) {
  red_flags <- c(
    red_flags,
    "Link uses HTTP instead of HTTPS"
  )
}

# Check urgency
urgent_words <- c(
  "urgent",
  "immediately",
  "act now",
  "within 24 hours"
)

for (word in urgent_words) {
  if (grepl(word, text, fixed = TRUE)) {
    red_flags <- c(
      red_flags,
      paste("Urgent/threatening language:", word)
    )
  }
}

# Check sensitive information
sensitive_words <- c(
  "password",
  "otp",
  "cvv",
  "pin",
  "credit card",
  "debit card",
  "bank account"
)

for (word in sensitive_words) {
  if (grepl(word, text, fixed = TRUE)) {
    red_flags <- c(
      red_flags,
      paste("Sensitive information mentioned:", word)
    )
  }
}

# Remove duplicate flags
red_flags <- unique(red_flags)

# Calculate risk
risk_score <- length(red_flags)

if (risk_score == 0) {
  risk_level <- "LOW RISK"
} else if (risk_score <= 3) {
  risk_level <- "MEDIUM RISK"
} else {
  risk_level <- "HIGH RISK"
}

# Display result
cat("\n============================================\n")
cat("              ANALYSIS RESULT\n")
cat("============================================\n")

cat("\nRisk Level :", risk_level)
cat("\nRisk Score :", risk_score, "\n")

if (risk_score > 0) {

  cat("\nRED FLAGS FOUND:\n")

  for (i in seq_along(red_flags)) {
    cat(i, ".", red_flags[i], "\n")
  }

  cat("\nWHY IS THIS MESSAGE UNSAFE?\n")
  cat("The message contains indicators commonly associated")
  cat(" with phishing attacks.\n")

  cat("\nRECOMMENDATION:\n")
  cat("Do not click suspicious links or share passwords,")
  cat(" OTPs, PINs or banking information.\n")

} else {

  cat("\nNo obvious phishing indicators were detected.\n")
  cat("Still verify the sender before trusting the message.\n")
}

cat("\n============================================\n")
cat("             END OF ANALYSIS\n")
cat("============================================\n")
