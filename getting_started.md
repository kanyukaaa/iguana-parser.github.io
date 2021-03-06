---
layout: base
---

<script type="text/javascript">
    $('body').scrollspy({
        target: '.bs-docs-sidebar',
        offset: 40
    });

    $("#sidebar").affix({
        offset: {
          top: 60
        }
    });
</script>

<div class="row">
    <!--Nav Bar -->
    <nav class="col-xs-3 bs-docs-sidebar">
        <ul id="sidebar" class="nav nav-stacked fixed">
            <li><a href="#Running">Running Iguana</a></li>
            <li>
                <a href="#Examples">Examples</a>
                <ul class="nav nav-stacked">
                    <li><a href="#XML">XML elements</a></li>
                    <li><a href="#OperatorePrecedence">Operator precedence</a></li>
                    <li><a href="#Haskell">Indentation rules</a></li>                
                </ul>
            </li>
        </ul>
    </nav>
    <!--Main Content -->
    <div class="col-xs-9">
        <section id="Running" class="group">
            {% include_relative examples/running.md %}
        </section>
        <section id="Examples" class="group">
            <h2>Examples</h2>
            Now we give some examples of using Iguana. The source code
            of this examples is available <a href="https://github.com/iguana-parser/examples">here</a>.</p>
            <div id="XML" class="subgroup">
                {% include_relative examples/xml.md %}
            </div>
            <div id="OperatorePrecedence" class="group">
                {% include_relative examples/operator_precedence.md %}
            </div>    
            <div id="Haskell" class="group">
                {% include_relative examples/haskell.md %}
            </div>            
        </section>
    </div>
</div>
