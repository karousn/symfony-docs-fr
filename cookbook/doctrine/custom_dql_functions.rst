Définir des Fonctions DQL Personnalisées
========================================

Doctrine vous permet de spécifier des fonctions DQL personnalisées. Pour plus
d'informations à ce sujet, lisez l'article du cookbook de Doctrine
« `Fonctions DQL définies par l'utilisateur`_ ».

Dans Symfony, vous pouvez définir vos fonctions DQL personnalisées comme suit :

.. configuration-block::

    .. code-block:: yaml

        # app/config/config.yml
        doctrine:
            orm:
                # ...
                entity_managers:
                    default:
                        # ...
                        dql:
                            string_functions:
                                test_string: Acme\HelloBundle\DQL\StringFunction
                                second_string: Acme\HelloBundle\DQL\SecondStringFunction
                            numeric_functions:
                                test_numeric: Acme\HelloBundle\DQL\NumericFunction
                            datetime_functions:
                                test_datetime: Acme\HelloBundle\DQL\DatetimeFunction

    .. code-block:: xml

        <!-- app/config/config.xml -->
        <container xmlns="http://symfony.com/schema/dic/services"
            xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
            xmlns:doctrine="http://symfony.com/schema/dic/doctrine"
            xsi:schemaLocation="http://symfony.com/schema/dic/services http://symfony.com/schema/dic/services/services-1.0.xsd
                                http://symfony.com/schema/dic/doctrine http://symfony.com/schema/dic/doctrine/doctrine-1.0.xsd">

            <doctrine:config>
                <doctrine:orm>
                    <!-- ... -->
                    <doctrine:entity-manager name="default">
                        <!-- ... -->
                        <doctrine:dql>
                            <doctrine:string-function name="test_string>Acme\HelloBundle\DQL\StringFunction</doctrine:string-function>
                            <doctrine:string-function name="second_string>Acme\HelloBundle\DQL\SecondStringFunction</doctrine:string-function>
                            <doctrine:numeric-function name="test_numeric>Acme\HelloBundle\DQL\NumericFunction</doctrine:numeric-function>
                            <doctrine:datetime-function name="test_datetime>Acme\HelloBundle\DQL\DatetimeFunction</doctrine:datetime-function>
                        </doctrine:dql>
                    </doctrine:entity-manager>
                </doctrine:orm>
            </doctrine:config>
        </container>

    .. code-block:: php

        // app/config/config.php
        $container->loadFromExtension('doctrine', array(
            'orm' => array(
                // ...
                'entity_managers' => array(
                    'default' => array(
                        // ...
                        'dql' => array(
                            'string_functions' => array(
                                'test_string'   => 'Acme\HelloBundle\DQL\StringFunction',
                                'second_string' => 'Acme\HelloBundle\DQL\SecondStringFunction',
                            ),
                            'numeric_functions' => array(
                                'test_numeric' => 'Acme\HelloBundle\DQL\NumericFunction',
                            ),
                            'datetime_functions' => array(
                                'test_datetime' => 'Acme\HelloBundle\DQL\DatetimeFunction',
                            ),
                        ),
                    ),
                ),
            ),
        ));

.. _`Fonctions DQL définies par l'utilisateur`: http://docs.doctrine-project.org/projects/doctrine-orm/en/latest/cookbook/dql-user-defined-functions.html