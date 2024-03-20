# R-PROJECT-
# Define movie options
movies <- c("Avengers: Endgame", "The Shawshank Redemption", "Inception", "The Godfather", "Pulp Fiction")

# Display movie options
cat("Welcome to Cinema Selector!\n")
cat("Choose a movie by entering its corresponding number:\n")
for (i in 1:length(movies)) {
  cat(i, ": ", movies[i], "\n")
}

# Get user input for movie selection
selection <- as.numeric(readline(prompt = "Enter the number of the movie you want to watch: "))

# Validate user input and display output
if (is.na(selection) || selection < 1 || selection > length(movies)) {
  cat("Invalid selection. Please enter a number corresponding to the movie.\n")
} else {
  cat("Enjoy watching", movies[selection], "!\n")
} 
