library(httr2)

# Killed in Gaza
# Connect to API and download data
resp <- httr2::request("https://data.techforpalestine.org/api/v2/") |> 
  # Then we location on path
  httr2::req_url_path_append("killed-in-gaza.min.json") |> 
  httr2::req_perform()

# transform to df
df <- resp |>
  httr2::resp_body_json(check_type = FALSE, 
                        simplifyVector = TRUE) 
