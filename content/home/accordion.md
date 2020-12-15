+++
widget = "blank"  # See https://sourcethemes.com/academic/docs/page-builder/
headless = true  # This file represents a page section.
active = true  # Activate this widget? true/false
weight = 40  # Order that this section will appear.

[design]
  # Choose how many columns the section has. Valid values: 1 or 2.
  columns = "1"

[design.background]
  # Apply a background color, gradient, or image.
  #   Uncomment (by removing `#`) an option to apply it.
  #   Choose a light or dark text color by setting `text_color_light`.
  #   Any HTML color name or Hex value is valid.

  # Background color.
  color = "gray"

  # Background gradient.
  # gradient_start = "DeepSkyBlue"
  # gradient_end = "SkyBlue"

  # Text color (true=light or false=dark).
  # text_color_light = "true"

[design.spacing]
  # Customize the section spacing. Order is top, right, bottom, left.
  padding = ["20px", "0", "0", "0"]

+++

<div class="accordion" id="myAccordion">
    <div class="card">
        <div class="card-header" id="headingOne">
            <p class="mb-0">
                <button type="button" class="btn accordion-title" data-toggle="collapse" data-target="#collapseOne">About</button>
            </p>
        </div>
        <div id="collapseOne" class="collapse" aria-labelledby="headingOne" data-parent="#myAccordion">
            <div class="card-body">
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer non dolor ut metus dapibus malesuada. Donec posuere porttitor felis vulputate feugiat. Quisque id odio vel neque sagittis molestie ac eu tortor. Donec eu sem et odio placerat faucibus in vitae ipsum. Nam ac velit ac neque cursus rutrum quis in nulla. <a href="/modeling">Learn more.</a></p>
            </div>
        </div>
    </div>
    <div class="card">
        <div class="card-header" id="headingTwo">
            <p class="mb-0">
                <button type="button" class="btn accordion-title" data-toggle="collapse" data-target="#collapseTwo">Projects</button>
            </p>
        </div>
        <div id="collapseTwo" class="collapse" aria-labelledby="headingTwo" data-parent="#myAccordion">
            <div class="card-body">
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer non dolor ut metus dapibus malesuada. Donec posuere porttitor felis vulputate feugiat. Quisque id odio vel neque sagittis molestie ac eu tortor. Donec eu sem et odio placerat faucibus in vitae ipsum. Nam ac velit ac neque cursus rutrum quis in nulla. <a href="/analysis">Learn more.</a></p>
            </div>
        </div>
    </div>
    <div class="card">
        <div class="card-header" id="headingThree">
            <p class="mb-0">
                <button type="button" class="btn accordion-title" data-toggle="collapse" data-target="#collapseThree">Resources</button>
            </p>
        </div>
        <div id="collapseThree" class="collapse" aria-labelledby="headingThree" data-parent="#myAccordion">
            <div class="card-body">
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer non dolor ut metus dapibus malesuada. Donec posuere porttitor felis vulputate feugiat. Quisque id odio vel neque sagittis molestie ac eu tortor. Donec eu sem et odio placerat faucibus in vitae ipsum. Nam ac velit ac neque cursus rutrum quis in nulla. <a href="/data">Learn more.</a></p>
            </div>
        </div>
    </div>
    <div class="card">
        <div class="card-header" id="headingTwo">
            <p class="mb-0">
                <button type="button" class="btn accordion-title" data-toggle="collapse" data-target="#collapseFour">People</button>
            </p>
        </div>
        <div id="collapseFour" class="collapse" aria-labelledby="headingFour" data-parent="#myAccordion">
            <div class="card-body">
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer non dolor ut metus dapibus malesuada. Donec posuere porttitor felis vulputate feugiat. Quisque id odio vel neque sagittis molestie ac eu tortor. Donec eu sem et odio placerat faucibus in vitae ipsum. Nam ac velit ac neque cursus rutrum quis in nulla. <a href="/analysis">Learn more.</a></p>
            </div>
        </div>
    </div>
</div>

<script>
$(document).ready(function(){
    // Add minus icon for collapse element which is open by default
    $(".collapse.show").each(function(){
        $(this).prev(".card-header").find(".fa").addClass("fa-minus").removeClass("fa-plus");
    });

    // Toggle plus minus icon on show hide of collapse element
    $(".collapse").on('show.bs.collapse', function(){
        $(this).prev(".card-header").find(".fa").removeClass("fa-plus").addClass("fa-minus");
    }).on('hide.bs.collapse', function(){
        $(this).prev(".card-header").find(".fa").removeClass("fa-minus").addClass("fa-plus");
    });
});
</script>
