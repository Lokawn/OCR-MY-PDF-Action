# OCR-MY-PDF-Action

<div align="center">
A turn scanned PDF's from URL into searchable documents

## Example and usage

Example of non-searchable [PDF file](.github/example_pdfs/Non-text-searchable.pdf) turned into a searchable [PDF file](.github/example_pdfs/output_searchable.pdf)


<details>
<summary>How to use this action</summary>
<br><br>     


<details>
<summary>Workflow Example(s) / Usage </summary>

<br><br>

<details>
<summary> View Example <b>Workflow Usage</b></summary> 
<br><br>

    - uses: actions/checkout@v2
    - uses: MarketingPipeline/OCR-PDF-Action@main
      with:
        # Define the input & output PDF file paths.
        input_file: .github/example_pdfs/Non-text-searchable.pdf
        output_file: .github/example_pdfs/output_searchable.pdf
        
    - name: Commit and Push PDF File
      run: |
         git config --global user.name "github-actions[bot]"
         git config --global user.email "41898282+github-actions[bot]@users.noreply.github.com"
         git add -A
         git commit -m "Added OCR PDF"
         git push
         
</details>

<br>

Example [workflow file](.github/workflows/example_workflow.yaml)         

</details>

<br>

### Workflow Options:


<table>
            <tr>
              <th>Inputs</th>
              <th>Meaning</th>
              <th>Default</th>
	      <th>Required</th>	    	    
            </tr>
            <tr>
              <td>input_file</td>
              <td>The file path to the input PDF</td>
              <td><code>undefined</code></td>
	      <td>Yes</td>	    
            </tr>         
	 <tr>
              <td>output_file</td>
              <td>The path to put the output PDF file</td>
              <td><code>undefined</code></td>
	      <td>Yes</td>	    
            </tr>         
	</table>         
	
<b><i>Note:</b></i> The output folder MUST exist.
	


<br><br>

</details>


</details>

See also the list of
[contributors](https://github.com/MarketingPipeline/OCR-PDF-Action/graphs/contributors) who
participate in this project.

This project is licensed under the MIT License - see the
[LICENSE.md](https://github.com/MarketingPipeline/OCR-PDF-Action/blob/main/LICENSE) file for
details.
